# Chapitre 08 - Supervision à l'échelle

<div class="meta-grid">
    <!-- Colonne de gauche -->

<!-- Auteurs -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-users"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Auteurs</div>
                <div class="meta-value">
                    Markov Grey & Charbel-Raphael Segerie
                </div>
            </div>
        </div>
        
        <!-- Affiliations -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-building"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Affiliations</div>
                <div class="meta-value meta-list">
                    <div><div>Centre français pour la sécurité de l'IA (CeSIA)</div></div>
                </div>
            </div>
        </div>

<!-- Section des Remerciements -->
<div class="meta-item">
    <span class="meta-icon">
        <i class="fas fa-heart"></i>
    </span>
    <div class="meta-content">
        <div class="meta-label">Remerciements</div>
        <div class="meta-value">
            Jeanne Salle, Chris Gerrby, Sebastian Gil, Josh Thorsteinson, Nicolas Guillard, Mateusz Bagiński, Yoann Poupart, Clément Dumas, Amaury Lorin, Mateo Rendon, Lucas Eichorn, Bogdan Ionut Cirstea, Gurvan R.
        </div>
    </div>
</div>
    </div>

    <!-- Colonne de droite -->
    <div class="meta-col">
        <!-- Date -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-calendar"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Dernière mise à jour</div>
                <div class="meta-value">2024-07-01</div>
            </div>
        </div>
        
        <!-- Temps de lecture -->
		<div class="meta-item">
			<span class="meta-icon">
				<i class="fas fa-clock"></i>
			</span>
			<div class="meta-content">
				<div class="meta-label">Temps de lecture</div>
				<div class="meta-value">85 min (cœur)</div>
			</div>
		</div>
        
        <!-- Liens -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-link"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Également disponible sur</div>
                <div class="meta-value meta-links">
                    <a href="https://docs.google.com/document/d/1k6rlyBCZJw8xbUx0dzd-4sOhlzj-xzsmwi_OIZY1-3M/edit?usp=sharing" class="meta-link">Google Docs</a>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="action-buttons">
    <div class="action-button disabled" data-tippy-content="Vidéo à venir">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <div class="action-button disabled" data-tippy-content="Audio à venir">
        <i class="fas fa-headphones"></i>
        <span>Écouter</span>
    </div>
    <div class="action-button disabled" data-tippy-content="PDF à venir">
        <i class="fas fa-file-pdf"></i>
        <span>Télécharger</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Commentaires</span>
    </a>
    <a href="https://docs.google.com/document/d/1DaygDSW0L5dWuJnpSjYPF2XUbW51UoBJsT1cjLYKc2w/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Contribuer</span>
    </div>

# Introduction

**Supervision**. À mesure que les systèmes d'IA deviennent de plus en plus capables, garantir leur alignement sur les valeurs et les intentions humaines devient un défi critique. Cette section introduit la supervision à l'échelle comme une approche cruciale pour maintenir le contrôle sur les IA avancées. Elle explique les problèmes auxquels nous sommes confrontés dans la génération de signaux d'entraînement pour des tâches complexes et « floues », et la nécessité de nouvelles méthodes pour fournir des retours précis. Cela est important, notamment lorsque les modèles d'IA commencent à effectuer des tâches dépassant l'expertise humaine. La section explore également le concept selon lequel la vérification est plus facile que la génération, expliquant pourquoi cette propriété est fondamentale pour les techniques de supervision à l'échelle.

**Décomposition des tâches**. S'appuyant sur le besoin de meilleures méthodes de supervision, la section suivante explore la décomposition des tâches comme une stratégie clé. La décomposition des tâches consiste à diviser des tâches complexes en sous-tâches plus petites et gérables, qui peuvent être récursivement subdivisées. Cette approche aide à générer de meilleurs signaux d'entraînement en simplifiant la tâche que nous devons évaluer et vérifier. La cognition factorielle étend ce concept pour répliquer la pensée humaine dans les modèles d'apprentissage automatique (ML) en décomposant le raisonnement, les tâches cognitives complexes.

**Supervision du processus**. Une autre façon d'aider à la supervision à l'échelle est de traiter certaines limites des approches basées sur les résultats. Cette section introduit le concept de supervision basée sur le processus. Nous expliquons la supervision du raisonnement externalisé (ERO) et le clonage procédural comme exemples spécifiques. Les techniques d'ERO comme la chaîne de pensée (CoT) encouragent les modèles de langage à « penser à voix haute », rendant leurs processus de raisonnement transparents pour une meilleure supervision et prévenant potentiellement des comportements indésirables. Le clonage procédural, une extension du clonage comportemental, vise à répliquer non seulement les actions finales mais l'ensemble du processus de prise de décision des experts. Ces méthodes offrent une approche plus fondée de la supervision en se concentrant sur le processus de raisonnement de l'IA plutôt que sur ses seules sorties.

**Amplification Itérée (Iterated Amplification, IA)**. S'appuyant sur les concepts de décomposition des tâches et de supervision du processus, cette section décrit l'amplification et la distillation. L'amplification améliore les capacités des superviseurs à résoudre des tâches plus complexes, tandis que la distillation traite les limites de l'amplification, telles que la complexité et l'utilisation des ressources. Ces processus sont combinés dans la Distillation et Amplification Itérées (IDA, de l'anglais *Iterated Distillation and Amplification*), une méthode visant à générer progressivement de meilleurs signaux d'entraînement pour des tâches difficiles à évaluer directement.

**Débat**. Cette section explore la sécurité de l'IA via le débat comme une technique d'opposition pour une supervision à l'échelle. Elle décrit comment des modèles d'IA défendant différentes positions, avec un juge humain ou IA déterminant le vainqueur, peut conduire à des résultats plus véridiques. Le potentiel du débat pour révéler des connaissances implicites, améliorer le raisonnement et renforcer notre capacité à superviser des systèmes d'IA complexes est analysé. Des métriques clés telles que l'écart critique du discriminateur (DCG, de l'anglais *Discriminator Critique Gap*) sont introduites, ainsi que les défis de l'arbitrage des débats. La section examine également les hypothèses requises pour que le débat converge vers la vérité.

**Faible-à-Fort (Weak-to-Strong, W2S)**. La section finale introduit la Généralisation Faible-à-Fort (W2SG, de l'anglais *Weak-to-Strong Generalization*) comme une approche pratique de supervision à l'échelle, s'appuyant sur les perspectives des techniques précédentes. Elle explique comment des modèles étroitement surhumains peuvent être utilisés comme études de cas pour les techniques de supervision à l'échelle. La W2SG implique l'entraînement de modèles d'IA forts en utilisant une supervision faible, visant à ce que le modèle fort surpasse son superviseur faible en exploitant des connaissances préexistantes. La section conclut en discutant de diverses méthodes d'évaluation des techniques de supervision, y compris les évaluations par encadrement et les évaluations méta-niveau adverses, offrant un moyen de juger les futurs protocoles de supervision à l'échelle.