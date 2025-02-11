# Chapitre 06 - Spécification

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

<!-- Section des remerciements -->
<div class="meta-item">
    <span class="meta-icon">
        <i class="fas fa-heart"></i>
    </span>
    <div class="meta-content">
        <div class="meta-label">Remerciements</div>
        <div class="meta-value">
            Jeanne Salle, Oscar Heitmann, Ram Rachum, Nicolas Guillard, Camille Berger
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
                <div class="meta-value">2023-12-01</div>
            </div>
        </div>
        
        <!-- Temps de lecture -->
		<div class="meta-item">
			<span class="meta-icon">
				<i class="fas fa-clock"></i>
			</span>
			<div class="meta-content">
				<div class="meta-label">Temps de lecture</div>
				<div class="meta-value">59 min (principal)</div>
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
                    <a href="https://www.lesswrong.com/s/3ni2P2GZzBvNebWYZ/p/mMBoPnFrFqQJKzDsZ" class="meta-link">Alignment Forum</a> · <a href="https://docs.google.com/document/d/1kEdmyVTUG3MO7lwuw4utHEm7CcavvgAiUZcWHaOZuPY/edit?usp=sharing" class="meta-link">Google Docs</a>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="action-buttons">
    <div class="action-button disabled" data-tippy-content="Vidéo à venir bientôt">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <div class="action-button disabled" data-tippy-content="Audio à venir bientôt">
        <i class="fas fa-headphones"></i>
        <span>Écouter</span>
    </div>
    <div class="action-button disabled" data-tippy-content="PDF à venir bientôt">
        <i class="fas fa-file-pdf"></i>
        <span>Télécharger</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Commentaires</span>
    </a>
    <a href="https://docs.google.com/document/d/1JfmzGii5QG6hW8AM5WxzDBVyGc14aLV_Lc_1PkK2ZLc/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Collaborer</span>
    </a>
</div>

# Introduction

**Apprentissage par renforcement** : Le chapitre commence par un rappel de certains concepts de l'apprentissage par renforcement. Il comprend un bref aperçu du concept de récompenses et de fonctions de récompense. Cette section pose les bases pour expliquer pourquoi la conception des récompenses est extrêmement importante.

**Optimisation** : Cette section introduit brièvement le concept de la loi de Goodhart. Elle fournit quelques motivations pour comprendre pourquoi les récompenses sont difficiles à spécifier de manière à ce qu'elles ne s'effondrent pas face à une pression d'optimisation immense.

**Mauvaise spécification des récompenses** : Après avoir bien saisi la notion de récompenses et d'optimisation, les lecteurs sont introduits à l'un des défis centraux de l'alignement des systèmes d'IA - la mauvaise spécification des récompenses. Ce problème, également connu sous le nom de problème d'alignement externe, commence par souligner la nécessité d'une conception rigoureuse des récompenses, au-delà de la simple conception algorithmique. La section présente ensuite des exemples concrets d'échecs de spécification des récompenses, tels que le détournement de récompense et l'altération de récompense.

**Apprentissage par imitation** : Cette section se concentre sur certaines solutions proposées à la mauvaise spécification des récompenses qui reposent sur l'apprentissage des fonctions de récompense en imitant le comportement humain. Elle examine des propositions telles que l'apprentissage par imitation (IL), le clonage comportemental (BC), et l'apprentissage par inversion de la récompense (IRL). Chaque section contient également un examen des problèmes et limitations potentiels de ces approches en ce qui concerne la résolution du détournement de récompense.

**Apprentissage par retours** : La section finale examine les propositions visant à corriger la mauvaise spécification des récompenses en fournissant des retours aux modèles d'apprentissage automatique. La section offre également un aperçu complet de la façon dont les grands modèles de langage actuels (LLM, de l'anglais Large Language Models) sont entraînés. La discussion couvre la modélisation de la récompense, l'apprentissage par renforcement à partir de retours humains (RLHF), l'apprentissage par renforcement à partir de retours artificiels (RLAIF), et les limites de ces approches.