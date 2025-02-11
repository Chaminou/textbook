# Chapitre 02 - Risques

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
            Jeanne Salle, Charles Martinet, Vincent Corruble, Sebastian Gil, Alejandro Acelas, Evander Hammer, Mo Munem, Mateo Rendon, Kieron Kretschmar, Camille Berger
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
				<div class="meta-value">122 min (partie principale), 11 min (annexe)</div>
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
                    <a href="https://docs.google.com/document/d/1ifYc49Wq-9HuqCXCa8jIr5n6ZOYjZ3FvxE9vHPMcu58/edit?usp=sharing" class="meta-link">Google Docs</a>
                </div>
            </div>
        </div>
    </div>
</div>

<div class="action-buttons">
   <a href="https://www.youtube.com/watch?v=dhr4u-w75aQ" class="action-button">
       <i class="fas fa-video"></i>
       <span>Regarder</span>
   </a>
   <div class="action-button disabled" data-tippy-content="Bientôt disponible">
       <i class="fas fa-headphones"></i>
       <span>Écouter</span>
   </div>
   <a href="https://raw.githubusercontent.com/CentreSecuriteIA/textbook/main/latex/AI%20Safety%20Atlas%20-%20Risks.pdf" class="action-button" download>
       <i class="fas fa-file-pdf"></i>
       <span>Télécharger</span>
   </a>
   <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
       <i class="fas fa-comment"></i>
       <span>Commentaires</span>
   </a>
   <a href="https://docs.google.com/document/d/1evE1rG91DKBuKlWnqPw45QtPxKBz0GlD_ZYrurNdvN4/edit?usp=sharing" class="action-button">
       <i class="fas fa-users"></i>
       <span>Animer</span>
   </a>
</div>

# Introduction

<figure class="video-figure" markdown="span">
<iframe style="width: 100%; aspect-ratio: 16 / 9;" frameborder="0" allowfullscreen src="https://www.youtube.com/embed/dhr4u-w75aQ"></iframe>
  <figcaption markdown="1"><b>Vidéo 2.1 :</b> Vidéo optionnelle pour avoir un aperçu des Risques.</figcaption>
</figure>

Le chapitre précédent a exploré des tendances comme l'accès aux ressources de calcul, la disponibilité des données, l'échafaudage des modèles existants et l'amélioration de l'efficacité des algorithmes. D'après ces tendances, nous pouvons supposer que les capacités de l'IA continueront de progresser dans les années à venir. Mais une question cruciale demeure : en quoi cette progression constante des capacités pourrait-elle représenter un réel défi ?

L'augmentation des capacités est problématique, car plus les modèles d'IA deviennent performants, plus l'échelle des risques potentiels s'élève.

La première étape consiste à comprendre - Quels sont exactement les scénarios préoccupants ? Quelles sont les probabilités que certains résultats néfastes se produisent plutôt que d'autres ? Et quels aspects du développement actuel de l'IA accélèrent ces risques ? Dans ce chapitre, nous visons à aborder ces questions fondamentales et à fournir un aperçu concret des divers risques dans le paysage de l'IA.

<figure markdown="span">
![Entrer une description alternative de l'image](Images/F2p_Image_1.png){ loading=lazy }
  <figcaption markdown="1"><b>Figure 2.1 :</b> La vision bidimensionnelle de la performance x généralité. Avec l'augmentation des capacités et de la généralité, nous observons également une augmentation des risques. Selon la trajectoire de développement et le takeoff, nous pourrions voir des périodes plus longues avec des risques potentiellement catastrophiques, ou des risques existentiels sévères émergeant soudainement. Les courbes et les couleurs de ce diagramme sont destinées à être illustratives et ne représentent pas une trajectoire de développement spécifiquement prévue.</figcaption>
</figure>

Nous avons déjà identifié plusieurs moyens par lesquels l'IA peut être utilisée de manière détournée. Cette utilisation abusive peut conduire à des résultats catastrophiques susceptibles d'impacter profondément la société. Au-delà de ce mésusage, nous approchons d'un seuil critique où le développement de capacités dangereusement avancées - comme la prolifération incontrôlée et les agents d'IA auto-réplicants - devient une réalité tangible. Ces capacités pourraient engendrer des scénarios où les systèmes d'IA s'étendent et évoluent rapidement, échappant au contrôle humain et provoquant potentiellement des perturbations et des dommages généralisés. Cette proximité avec des capacités si avancées souligne l'urgence d'une vigilance et de mesures proactives. Qui plus est, le paysage réglementaire actuel présente des lacunes significatives, manquant de cadres exhaustifs régissant le développement et le déploiement de l'IA. Cette absence de réglementations adéquates ne fait qu'exacerber les risques inhérents à l'intelligence artificielle.

**Décomposition des Risques**. La première section propose une catégorisation des risques en trois groupes principaux : le mésusage, le désalignement et les risques systémiques. Les risques de mésusage concernent les situations où un individu ou un groupe utilise intentionnellement l'IA à des fins préjudiciables. Les risques de désalignement émergent des systèmes d'IA eux-mêmes, résultant de problèmes intrinsèques de conception, tels que des systèmes poursuivant des objectifs divergents des valeurs humaines. Les risques systémiques englobent des problématiques plus larges qui surgissent lorsqu'on considère un système d'IA non pas isolément, mais comme une variable au sein d'interactions globales impliquant les incitations de systèmes complexes – politique, société, économie – où aucune entité n'endosse une responsabilité unique. Au-delà de la categorisation des sources de risques, nous distinguons également différentes échelles de risque potentiel : les risques catastrophiques, causant un préjudice à une large fraction de l'humanité, et les risques existentiels, dont la gravité pourrait compromettre la capacité de reconstruction de la civilisation humaine.

Les sections suivantes se concentreront à répondre aux questions suivantes : Quels sont exactement les risques ? Que se passe-t-il et de quoi sommes-nous préoccupés ?

**Capacités à Risque**. Nous commençons par explorer des capacités spécifiques de l'IA qui présentent des risques significatifs. Celles-ci incluent le potentiel d'utiliser l'IA pour développer des armes biologiques et commettre des délits cybernétiques, ainsi que sa capacité à la tromperie et à la manipulation. Nous considérons également les risques associés aux systèmes d'IA qui manifestent une capacité d'action autonome, une réplication indépendante et une conscience approfondie de leur environnement. Comprendre ces capacités est crucial pour développer des stratégies ciblées d'atténuation des risques.

En comprenant la nature et l'étendue de ces risques, nous pouvons développer des stratégies plus efficaces pour les atténuer et garantir que le développement de l'IA reste bénéfique pour l'humanité. Les chapitres suivants s'appuieront sur cette base, explorant de manière plus approfondie les risques spécifiques, les solutions techniques et les considérations politiques.