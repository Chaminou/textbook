# Atlas de la Sécurité de l'IA

<div class="chapter-meta">
<div class="meta-grid">
    <!-- Left Column -->
    <div class="meta-col">
        <!-- Authors -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-pen-nib"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Auteurs</div>
                <div class="meta-value meta-list">
                    <div>
                    <div>Markov Grey</div>
                    <div>Charbel-Raphael Segerie</div>
                    <div>Jeanne Salle</div>
                    <div>Charles Martinet</div>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- Affiliations -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-university"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Affiliations</div>
                <div class="meta-value meta-list">
                    <div><div>Centre Français pour la Sécurité de l'IA (CeSIA)</div></div>
                </div>
            </div>
        </div>

        <!-- Advisors section -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-graduation-cap"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Conseillers</div>
                <div class="meta-value">
                    <div>Vincent Corruble</div>
                </div>
            </div>
        </div>
    </div>

    <!-- Right Column -->
    <div class="meta-col">
        <!-- Citation -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-quote-right"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Citer ce travail</div>
                <div class="meta-value">
                    <div>Markov Grey et Charbel-Raphael Segerie et al. 2024. Atlas de la Sécurité de l'IA. Centre Français pour la Sécurité de l'IA (CeSIA). ai-safety-atlas.com</div>
                </div>
            </div>
        </div>

        <!-- Projet financé par -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-hand-holding-dollar"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Projet financé par</div>
                <div class="meta-value">
                    <div><a href="https://manifund.org/projects/ai-safety-textbook" target="_blank" style="text-decoration: none; color: inherit;">Ryan Kidd (Rétrocession Manifund)</a></div>
                    <div>Open Philanthropy</div>
                </div>
            </div>
        </div>

        <!-- Remerciements -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-heart"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Remerciements</div>
                <div class="meta-value">
                    <div>Jonathan Claybrough</div>
                    <div>Jérémy Andréoletti</div>
                    <div>Evander Hammer</div>
                    <div>Josh Thorsteinson</div>
                </div>
            </div>
        </div>
    </div>
</div>
</div>

<div style="content: ''; display: block; width: 100%; height: 3px; background-color: currentColor; opacity: 0.7; margin: 1.5em 0;"></div>

L'IA connaît une croissance sans précédent de ses capacités, passant de l'écriture de code et de l'analyse de publications scientifiques à la génération d'images et à la réalisation de raisonnements complexes. Alors que ces systèmes s'approchent rapidement et sont susceptibles de dépasser les performances humaines dans de nombreux domaines, les décisions que nous prenons aujourd'hui concernant leur développement façonneront l'avenir de l'humanité. Ce livre offre un cadre complet pour comprendre et relever les défis de la sécurité de l'IA - depuis les concepts fondamentaux jusqu'à leur mise en œuvre technique. Que vous soyez un décideur politique, un chercheur, un ingénieur ou un citoyen engagé, notre objectif est de vous fournir les connaissances nécessaires pour contribuer de manière significative à garantir que le développement de l'IA bénéficie à l'humanité.

!!! citation "Geoffrey Hinton (Informaticien le plus cité, Parrain de l'IA moderne, Lauréat du Prix Turing) ([Hinton, 2024](https://www.cbsnews.com/news/geoffrey-hinton-ai-dangers-60-minutes-transcript/))"

Je ne discerne aucune voie qui nous garantirait la sécurité. Nous entrons dans une période de grande incertitude où nous sommes confrontés à des défis totalement inédits. Et normalement, la première fois qu'on aborde quelque chose de complètement nouveau, on se trompe. Or, nous ne pouvons pas nous permettre l'erreur avec de tels enjeux.
[...]
Si l'on prend au sérieux le risque existentiel, comme je le fais désormais, il serait peut-être plus que raisonnable de simplement cesser tout développement ultérieur [...] c'est un peu comme si des extraterrestres avaient débarqué sans que personne ne le remarque, tant ils parlent parfaitement notre langue

## [Capacités](https://ai-safety-atlas.com/chapters/01/)

Pourquoi les IA pourraient continuer de s'développer de manière toujours plus générale et performante ?

Les modèles d'IA passent progressivement d'outils spécialisés à des systèmes de plus en plus polyvalents capables de gérer des tâches complexes. Dans ce chapitre, nous abordons les tendances empiriques montrant que le passage à l'échelle - en utilisant plus de données, de puissance de calcul et de paramètres - conduit à des gains constants en termes de capacités et de généralité. Nous expliquons les définitions de concepts tels que l'intelligence artificielle générale (IAG) et la superintelligence (IAS) que nous utiliserons tout au long de l'ouvrage. Plutôt que de considérer les progrès de l'IA à travers des seuils discrets comme l'intelligence « étroite » contre « générale », nous introduisons des cadres pour mesurer les capacités, la généralité et l'autonomie le long de courbes continues. Sur cette base, nous examinons les arguments pour différents scénarios de takeoff de l'IA et fournissons des opinions d'experts sur les délais menant à une IA transformatrice. Comprendre ces concepts structure les conversations autour des sources potentielles de risques et des stratégies de sécurité dans le reste de l'ouvrage. Après avoir lu ce chapitre, vous serez en mesure d'évaluer de manière critique de nombreuses affirmations sur les progrès de l'IA et de participer à des discussions éclairées sur les développements futurs de l'intelligence artificielle.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/01/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <a href="https://www.youtube.com/watch?v=J_iMeH1hb9M" class="action-button">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </a>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1L32xCVUCWEsm-x8UZ3GSTgKnmBcC7rJQLLIh9wGLj40/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Risques](https://ai-safety-atlas.com/chapters/02/)

Quels dangers peuvent surgir si l'IA continue de s'améliorer sans cesse ?

Une fois que nous avons établi les arguments centraux expliquant pourquoi les capacités, la généralité et l'autonomie pourraient continuer de progresser, nous pouvons examiner les risques correspondant à ces niveaux accrus. Nous divisons les risques liés à l'IA en trois catégories principales : la mauvaise utilisation (les humains utilisant l'IA pour nuire, comme les cyberattaques ou les armes biologiques), le désalignement (les systèmes d'IA échouant de manière imprévue), et les risques systémiques (problèmes émergeant lorsque l'IA interagit avec d'autres systèmes complexes). 

Nous abordons également les facteurs sous-jacents qui amplifient tous ces risques, tels que les pressions concurrentielles créant des dynamiques de course et le déploiement généralisé. Enfin, nous proposons des explications concrètes sur la façon d'appréhender des capacités potentiellement dangereuses : tromperie, conscience situationnelle, réplication autonome, comportements de complotage et de recherche de pouvoir. 

À la fin de ce chapitre, vous serez capable d'identifier comment différents risques émergent des défaillances techniques des systèmes d'IA, de la combinaison des capacités de l'IA avec les incitations humaines et d'autres systèmes socio-techniques complexes.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/02/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <a href="https://www.youtube.com/watch?v=dhr4u-w75aQ" class="action-button">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </a>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1evE1rG91DKBuKlWnqPw45QtPxKBz0GlD_ZYrurNdvN4/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Stratégies](https://ai-safety-atlas.com/chapters/03/)

Quelles stratégies pouvons-nous élaborer pour atténuer les risques ?

En s'appuyant sur la compréhension des capacités et des risques, ce chapitre examine les stratégies concrètes visant à atténuer ces risques et à rendre le développement de l'IA plus sûr. Nous divisons les stratégies potentielles d'atténuation en trois catégories correspondant aux risques : prévenir la mauvaise utilisation (par exemple via des API surveillées et des technologies défensives), traiter le désalignement (par exemple par des recherches techniques et des mesures de contrôle), et gérer les impacts systémiques (par exemple par la gouvernance et la culture de sécurité). Nous expliquons comment la Sécurité de l'IA commence tout juste à prendre de l'ampleur en tant que domaine, mais il est important de se rappeler qu'aucune solution unique ne pourrait être suffisante. Nous pourrions avoir besoin d'une approche par couches où plusieurs garde-fous travaillent ensemble pour créer une protection robuste contre les risques décrits dans le chapitre précédent. L'objectif de ce chapitre est de donner un aperçu de diverses stratégies et propositions de sécurité et de montrer comment ces différents éléments peuvent s'intégrer dans une vision plus large. En lisant ce chapitre et les précédents, vous disposez d'une base solide pour les approfondissements individuels qui suivent dans tous les chapitres ultérieurs. Les stratégies systémiques et sociales décrites conduisent directement aux prochains chapitres sur la gouvernance et les évaluations, et les problèmes techniques et les stratégies d'atténuation sont également discutés dans des chapitres individuels dédiés.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/03/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <a href="https://www.youtube.com/watch?v=iO7Jl4xders" class="action-button">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </a>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1cv0gzwSouDjckYHzV7gYbHPKhJZR6bwbJWgHzEJ604Q/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Gouvernance](https://ai-safety-atlas.com/chapters/04/)

Comment pouvons-nous guider le développement et le déploiement sûr de l'IA ?

Les chapitres précédents ont fourni des aperçus de ce que l'IA peut faire, de ce qui pourrait mal tourner et des stratégies d'atténuation potentielles. Dans ce chapitre, nous examinons plus en profondeur comment façonner l'impact de l'IA par le biais de cadres de gouvernance. Nous commençons par expliquer pourquoi la régulation de l'IA présente des défis uniques en raison de choses comme les bonds de capacités inattendus, les problèmes de sécurité post-déploiement et la prolifération rapide. Nous expliquons les cibles de gouvernance clés telles que - la gouvernance du calcul (contrôle des ressources essentielles comme les puces et les ressources d'entraînement), la gouvernance des données (gestion des données d'entraînement et du déploiement). Ensuite, nous examinons les différentes couches pouvant introduire des changements pour affecter les cibles choisies - la gouvernance d'entreprise (cadres de politique de mise à l'échelle responsable [RSP] comme ceux d'Anthropic), la gouvernance nationale (initiatives gouvernementales comme les Instituts de sécurité de l'IA et les réglementations comme le Règlement IA de l'Union européenne), et la gouvernance internationale (approches allant de la non-prolifération aux accords réglementaires). Réitérant ce que nous avons dit dans le chapitre sur les stratégies, aucune couche de gouvernance ne pourrait être complètement suffisante - nous avons plutôt besoin d'actions coordonnées à tous les niveaux pour traiter efficacement les risques liés à l'IA. La lecture de ce chapitre vous aidera à participer de manière significative aux discussions sur le développement, le déploiement, l'audit et la politique de l'IA.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/04/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <a href="https://www.youtube.com/watch?v=FSKuDqze9es" class="action-button">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </a>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1tp5rpzw_gekjju-UBp8tkbbnQOuA2QzsPF_um8Z4IOU/edit?tab=t.0#heading=h.fo57hwsn3del" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Évaluations](https://ai-safety-atlas.com/chapters/05/)

Comment pouvons-nous mesurer si un système d'IA est réellement sûr ?

Les évaluations constituent le premier chapitre de ce que nous considérons comme la séquence technique, car elles nous aident à faire le lien entre la théorie et la pratique en montrant comment les résultats des évaluations peuvent déclencher des actions de gouvernance spécifiques ou des protocoles de sécurité techniques. Notre explication se décompose selon les questions suivantes - que évaluons-nous ? (propriétés évaluées), comment l'évaluons-nous ? (techniques d'évaluation), et quels éléments interviennent dans de bonnes évaluations ? (conception de l'évaluation). Nous abordons les méthodes d'évaluation spécifiques à la sécurité de l'IA dans trois catégories différentes - évaluations des capacités dangereuses (ce que les systèmes d'IA peuvent faire), évaluations des propensions (leur tendance comportementale par défaut), et évaluations de contrôle (notre capacité à maintenir la sécurité dans des conditions adverses). Nous expliquons comment nous pourrions créer des techniques pour évaluer les capacités dangereuses (déception, risques nucléaires, radiologiques, biologiques et chimiques, et réplication autonome) et les propensions dangereuses (par exemple la recherche de pouvoir et la manipulation) que nous avions précédemment décrites dans le chapitre sur les risques. Après avoir lu ce chapitre, vous serez capable de comprendre ce que implique la conception d'évaluations de sécurité de l'IA, et comment leurs résultats peuvent alimenter à la fois les directions de recherche techniques et les décisions de gouvernance.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/05/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <div class="action-button disabled" data-tippy-content="Vidéo à venir">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1T-UU0FBeElX6cvbWYKpVAl3U4ivrQLHA3IdIWqWKuBA/edit?tab=t.0#heading=h.fo57hwsn3del" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Spécification](https://ai-safety-atlas.com/chapters/06/)

Pourquoi est-il si difficile de dire aux systèmes d'IA ce que nous voulons ?

Les évaluations nous aident à comprendre ce que les systèmes d'IA peuvent faire ou ont tendance à faire, et si nos mesures d'atténuation actuelles sont suffisantes. L'étape suivante consiste à essayer de répondre - comment spécifions-nous correctement ce que nous voulons que l'IA fasse dès le départ ? Nous avons introduit le concept général de détournement des spécifications dans le chapitre sur les risques, ici nous développons ce concept et examinons les fondements théoriques et les modes d'échec pratiques comme le détournement de récompense (trouver des moyens non intentionnels de maximiser la récompense) et la manipulation de récompense (manipulation directe des mécanismes de récompense). Nous expliquons également comment les stratégies d'atténuation proposées au problème de spécification pourraient fonctionner. Cela comprend des méthodes basées sur l'imitation (par exemple, le clonage comportemental, l'apprentissage par inversion de récompense) et des approches basées sur les retours (par exemple, la modélisation de récompense, l'apprentissage par renforcement à partir des retours humains (RLHF, de l'anglais *Reinforcement Learning from Human Feedback*), l'IA constitutionnelle). Nous abordons également les limites de ces approches qui aident à établir le contexte des prochains chapitres sur la généralisation et la supervision à grande échelle. Après avoir lu ce chapitre, vous serez capable de comprendre pourquoi essayer d'encoder même des instructions simples peut conduire à des comportements inattendus et comment la recherche sur la sécurité de l'IA tente actuellement de relever ces défis.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/06/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <div class="action-button disabled" data-tippy-content="Vidéo à venir">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1JfmzGii5QG6hW8AM5WxzDBVyGc14aLV_Lc_1PkK2ZLc/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Généralisation](https://ai-safety-atlas.com/chapters/07/)

Pourquoi les IA pourraient-elles poursuivre des objectifs non intentionnels ?

Voici la traduction :

Dans ce chapitre, nous nous penchons sur la façon dont les systèmes d'IA apprennent et généralisent réellement à partir de leur entraînement. Nous commençons par un rappel de ce que signifient concrètement les "objectifs" d'une IA, et comment les personnes travaillant sur la sécurité de l'IA utilisent ce terme. Cela s'appuie sur l'intuition fournie dans les chapitres précédents sur les risques et les évaluations, distinguant les capacités (ce que les systèmes d'IA peuvent faire) des propensions (leur comportement par défaut). Nous vous guidons à travers la façon dont la généralisation des capacités et la généralisation des objectifs sont des choses distinctes, en utilisant des résultats empiriques concrets. Nous nous concentrons spécifiquement sur la mauvaise généralisation des objectifs, qui est différente des problèmes standard de généralisation en apprentissage automatique comme le surapprentissage. Nous explorons également pourquoi la mauvaise généralisation des objectifs se produit en examinant la théorie des paysages de perte des réseaux de neurones, qui montre comment différents types d'algorithmes peuvent émerger de différentes exécutions d'entraînement. Nous accordons une attention particulière à un type spécifique d'algorithme appris - un optimiseur appris. En utilisant le concept d'optimiseurs appris comme point de départ, nous approfondissons les problèmes d'alignement interne et d'alignement trompeur (manipulation) qui ont été mentionnés dans de nombreux chapitres précédents. Nous relions également ces préoccupations aux stratégies d'évaluation mentionnées précédemment, ainsi qu'aux stratégies d'atténuation qui seront explorées dans le chapitre suivant sur l'interprétabilité. À la fin de ce chapitre, vous devriez être capable de distinguer les différentes façons dont les modèles d'apprentissage automatique peuvent généraliser entre les distributions et comprendre comment et pourquoi des systèmes d'IA capables pourraient manipuler, tromper et poursuivre des objectifs non intentionnels à long terme.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/07/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <div class="action-button disabled" data-tippy-content="Vidéo à venir">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1uQooTncb7Hw2NhITtr3S5iGHqT6cvj74c0SZ4Unad_M/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Supervision à grande échelle](https://ai-safety-atlas.com/chapters/08/)

Comment pouvons-nous maintenir un contrôle significatif lorsque les IA sont plus intelligentes que nous ?

S'appuyant sur le problème de spécification exploré dans les chapitres précédents, nous examinons comment nous pourrions maintenir une supervision humaine significative même lorsque les tâches commencent à dépasser la capacité humaine à fournir des retours itératifs. Le défi principal est de fournir des signaux d'entraînement précis pour des tâches complexes et "floues" où les critères de succès sont ambigus et l'évaluation directe devient infaisable. Nous commençons par explorer comment décomposer des tâches hautement complexes en morceaux plus gérables à travers des techniques comme la décomposition de tâches. Nous expliquons ensuite des approches visant à extraire les connaissances latentes d'une IA par une supervision du raisonnement externalisé et un clonage procédural - des stratégies qui se concentrent sur l'alignement de l'ensemble du processus de raisonnement de l'IA plutôt que simplement ses sorties. Nous approfondissons des cadres théoriques comme l'amplification et la distillation itératives (IDA, de l'anglais Iterated Distillation and Amplification) et des approches plus pratiques comme le débat pour la sécurité de l'IA et la généralisation du faible au fort (W2S, de l'anglais Weak-to-Strong). Enfin, nous examinons des méthodes pour évaluer ces techniques de supervision, qui incluent des explications sur les expériences de sandwich et les évaluations adverses de niveau méta. À la fin de ce chapitre, vous devriez comprendre les stratégies existantes pour maintenir le contrôle sur des systèmes d'IA qui dépassent les capacités humaines.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/08/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <div class="action-button disabled" data-tippy-content="Vidéo à venir">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1DaygDSW0L5dWuJnpSjYPF2XUbW51UoBJsT1cjLYKc2w/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

## [Interprétabilité](https://ai-safety-atlas.com/chapters/09/)

Comment pouvons-nous comprendre ce qui se passe à l'intérieur des systèmes d'IA ?

Notre dernier chapitre examine comment nous pourrions décortiquer le fonctionnement interne des modèles d'IA. Les progrès en interprétabilité pourraient aider à résoudre de nombreux risques et défis abordés tout au long du livre - de la détection des comportements trompeurs à l'orientation et à la vérification des résultats d'entraînement. Nous nous concentrons principalement sur l'interprétabilité mécaniste - une approche ascendante qui vise à comprendre de l'intérieur les réseaux de neuronaux en étudiant comment leurs composants traitent l'information. Nous expliquons à la fois les méthodes observationnelles qui analysent les composants du modèle sans modification (comme la visualisation de caractéristiques et la sonde), et les méthodes interventionnelles qui testent et modifient activement le comportement du modèle (comme le [patching d'activations] et le [pilotage d'activations]). Nous examinons également quelques efforts pour automatiser et mettre à l'échelle l'interprétabilité à travers des techniques comme la découverte automatique de circuits (*[ACDC]).

Comme toutes les approches abordées dans ce livre - des cadres de gouvernance aux mesures de sécurité techniques - l'interprétabilité n'est qu'un outil dans notre boîte à outils de la sécurité de l'IA. Le chemin vers des systèmes d'IA plus sûrs nécessitera probablement de combiner des perspectives et des méthodes issues de toutes ces différentes approches. Bien que les techniques actuelles d'interprétabilité présentent des limitations significatives, elles représentent aussi certaines de nos meilleures tentatives pour comprendre ces systèmes de plus en plus complexes. Après avoir lu ce chapitre, vous comprendrez à la fois le potentiel et les limitations actuelles de ces outils, et comment ils pourraient contribuer à construire des systèmes d'IA plus sûrs à l'avenir.

<div class="action-buttons">
    <a href="https://ai-safety-atlas.com/chapters/09/" class="action-button">
        <i class="fas fa-book"></i>
        <span>Lire</span>
    </a>
    <div class="action-button disabled" data-tippy-content="Vidéo à venir">
        <i class="fas fa-video"></i>
        <span>Regarder</span>
    </div>
    <a href="https://forms.gle/ZsA4hEWUx1ZrtQLL9" class="action-button">
        <i class="fas fa-comment"></i>
        <span>Retour</span>
    </a>
    <a href="https://docs.google.com/document/d/1izDWZKR_xB2qj2a8LkbqcnqnjBIC-C7fn-74CIA-m9w/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Faciliter</span>
    </a>
</div>

# La Voie à Suivre

La sécurité de l'IA implique d'énormes défis techniques et de coordination sociale. En écrivant ce livre, nous espérons vous aider à rejoindre la communauté croissante de personnes travaillant sur ces problèmes. Que vous choisissiez de contribuer par la recherche technique, le travail politique, ou simplement en faisant connaître le sujet par des actions de sensibilisation, votre implication compte ! Chaque nouvel acteur travaillant sur ces problèmes nous rapproche de garantir que le développement de l'IA conduise à un avenir prospère pour l'humanité.