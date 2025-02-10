# Chapitre 01 - Capacités

<div class="meta-grid">
    <!-- Colonne de gauche -->
    <div class="meta-col">

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
                    <div><div>Centre Français pour la Sécurité de l'IA (CeSIA)</div></div>
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
            Jeanne Salle, Charles Martinet, Vincent Corruble, Diego Dorn, Josh Thorsteinson, Jonathan Claybrough, Alejandro Acelas, Jamie Raldua Veuthey, Alexandre Variengien, Léo Dana, Angélina Gentaz, Nicolas Guillard, Leo Karoubi
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
                <div class="meta-value">2024-11-20</div>
            </div>
        </div>
        
        <!-- Temps de lecture -->
		<div class="meta-item">
			<span class="meta-icon">
				<i class="fas fa-clock"></i>
			</span>
			<div class="meta-content">
				<div class="meta-label">Temps de lecture</div>
				<div class="meta-value">94 min (partie principale), 51 min (annexe)</div>
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
                    <a href="https://www.alignmentforum.org/posts/MkfaQyxB9PN4h8Bs9/" class="meta-link">Alignment Forum</a> · <a href="https://docs.google.com/document/d/1HKo0Kest9Xppjn7m2ODpfMUlEu93SzLsfxXBH48Xaus/edit?usp=sharing" class="meta-link">Google Docs</a>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="action-buttons">
   <a href="https://www.youtube.com/watch?v=J_iMeH1hb9M" class="action-button">
       <i class="fas fa-video"></i>
       <span>Regarder</span>
   </a>
   <div class="action-button disabled" data-tippy-content="Audio à venir prochainement">
       <i class="fas fa-headphones"></i>
       <span>Écouter</span>
   </div>
   <a href="https://raw.githubusercontent.com/CentreSecuriteIA/textbook/main/latex/AI%20Safety%20Atlas%20-%20Capabilities.pdf" class="action-button" download>
       <i class="fas fa-file-pdf"></i>
       <span>Télécharger</span>
   </a>
   <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
       <i class="fas fa-comment"></i>
       <span>Commentaires</span>
   </a>
   <a href="https://docs.google.com/document/d/1L32xCVUCWEsm-x8UZ3GSTgKnmBcC7rJQLLIh9wGLj40/edit?usp=sharing" class="action-button">
       <i class="fas fa-users"></i>
       <span>Collaborer</span>
   </a>
</div>

# Introduction

<figure class="video-figure" markdown="span">
<iframe style="width: 100%; aspect-ratio: 16 / 9;" frameborder="0" allowfullscreen src="https://www.youtube.com/embed/J_iMeH1hb9M"></iframe>
  <figcaption markdown="1"><b>Vidéo 1.1 :</b> Vidéo optionnelle pour avoir un aperçu des capacités de l'IA.</figcaption>
</figure>

!!! quote "Yann LeCun, scientifique en chef de l'IA chez Meta et lauréat du prix Turing, mai 2023 ([Heaven, 2023](https://www.technologyreview.com/2023/05/02/1072528/geoffrey-hinton-google-why-scared-ai/))"

Il est évident que les machines deviendront plus intelligentes que les humains dans tous les domaines où l'intelligence humaine s'exprime. Ce n'est qu'une question de temps et de modalités, nullement de possibilité.

Je suis prêt à traduire, mais je n'ai pas de texte source à traduire. Pourriez-vous me fournir le texte que vous voulez que je traduise ?

Le domaine de l'intelligence artificielle a connu une évolution spectaculaire ces dernières années. Ce chapitre établit les fondements de l'ensemble de l'ouvrage en définissant ce que les systèmes d'IA sont capables de faire actuellement, comment ils développent ces capacités, et comment nous pourrions envisager leur progression future. Cette compréhension est cruciale pour tous les chapitres suivants : la discussion des capacités dangereuses et des risques potentiels (Chapitre 2) découle directement de la compréhension des capacités. De même, les solutions techniques proposées (Chapitre 3) et les solutions de gouvernance (Chapitre 4) doivent nécessairement prendre en compte le présent et le futur projeté des capacités de l'IA.

<figure markdown="span">
![Enter image alt description](Images/XnK_Image_1.png){ loading=lazy }
  <figcaption markdown="1"><b>Figure 1.1 :</b> Nous expliquons d'abord les modèles de fondation, qui ont continuellement démontré des capacités améliorées grâce à leur mise à l'échelle. Nous examinons ensuite empiriquement les lois de mise à l'échelle. Sur la base de ces tendances, nous explorons quelques techniques que les chercheurs utilisent pour tenter de prédire les progrès futurs de l'IA.</figcaption>
</figure>

État de l'art de l'IA - Capacités révolutionnaires atteintes dans plusieurs domaines. Nous commençons par explorer comment les systèmes d'IA sont passés d'outils spécialisés et étroits à des outils de plus en plus polyvalents. Les modèles de langage peuvent désormais s'engager dans un raisonnement complexe, tandis que les systèmes de vision par ordinateur démontrent une compréhension sophistiquée des informations visuelles. En robotique, nous voyons émerger des systèmes capables d'apprendre et de s'adapter à des environnements réels avec une autonomie croissante. L'objectif de cette section est de donner au lecteur de nombreux exemples provenant de différents domaines illustrant l'accélération des capacités de l'IA.

**Modèles de fondation - Ont révolutionné la façon dont nous construisons les systèmes d'IA.** La section suivante explore comment nous sommes passés d'architectures plus petites et spécialisées à des architectures générales à grande échelle. Plutôt que de construire des systèmes séparés pour chaque tâche, ces modèles de fondation servent de point de départ. Ils sont des blocs de construction qui peuvent ensuite être adaptés à diverses applications par apprentissage fin (ou *fine-tuning*). Nous explorons comment ces modèles sont entraînés, leurs propriétés clés et les défis uniques qu'ils présentent. L'émergence de capacités inattendues de ces modèles soulève des questions importantes concernant leur potentiel et leurs implications pour la sécurité de l'IA.

**Comprendre l'Intelligence - Les capacités nécessitent une mesure précise pour guider le travail de sécurité**. L'objectif de cette section est de fournir une compréhension de ce que signifient en pratique des termes comme intelligence artificielle générale (IAG) et super-intelligence artificielle. À travers des études de cas détaillées et des observations empiriques, nous examinons différentes approches pour définir et mesurer les capacités de l'IA. Au-delà des distinctions binaires traditionnelles entre IA "étroite" et IA "générale", nous introduisons des cadres formels plus nuancés permettant de suivre l'évolution des capacités selon plusieurs dimensions, essentiels pour comprendre quand et comment des mesures de sécurité doivent être mises en œuvre.

**Mise à l'échelle - La leçon amère et les lois empiriques de mise à l'échelle montrent que l'échelle est moteur de progrès**. Nous explorons comment des algorithmes simples combinés à un calcul à grande échelle surpassent souvent des approches sophistiquées conçues manuellement. Cela nous conduit à examiner les lois de mise à l'échelle qui décrivent comment les performances de l'IA s'améliorent avec différentes variables telles que - les données, le nombre de paramètres et les ressources informatiques accrues. Cette section contient également un examen du débat portant sur la question de savoir si l'échelle seule suffit pour atteindre des capacités d'IA transformatives.

**Projection - Prédire les progrès des capacités nous aide à anticiper les dispositifs de sécurité**. En nous appuyant sur notre compréhension des capacités actuelles et des comportements de mise à l'échelle, nous examinons différentes approches pour anticiper les progrès futurs. Des ancres biologiques à l'analyse de tendances, nous explorons des cadres permettant de formuler des prédictions éclairées sur les trajectoires de développement de l'IA. Il est crucial de déterminer précisément quand et comment déployer différents mécanismes de sécurité.

**Annexes - Aperçu des opinions d'experts sur l'IA, débats détaillés autour de la mise à l'échelle et des tendances de mise à l'échelle.** Nous considérons ces sections comme optionnelles, mais toujours utiles pour ceux qui souhaitent approfondir un peu le sujet. Le chapitre se termine par des annexes examinant les opinions d'experts sur les progrès de l'IA, des discussions approfondies sur la nature et les limites des grands modèles de langage, et des données exhaustives sur les tendances clés du développement de l'IA.