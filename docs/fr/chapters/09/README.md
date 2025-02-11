# Interprétabilité

<div class="chapter-meta">

<div class="meta-grid">
    <!-- Left Column -->
    <div class="meta-col">

        <!-- Auteurs -->
        <div class="meta-item">
            <span class="meta-icon">
                <i class="fas fa-users"></i>
            </span>
            <div class="meta-content">
                <div class="meta-label">Auteurs</div>
                <div class="meta-value">
                    Jeanne Salle & Charbel-Raphael Segerie
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
            Markov Grey
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
                <div class="meta-value">2024-11-01</div>
            </div>
        </div>
        
        <!-- Temps de lecture -->
		<div class="meta-item">
			<span class="meta-icon">
				<i class="fas fa-clock"></i>
			</span>
			<div class="meta-content">
				<div class="meta-label">Temps de lecture</div>
				<div class="meta-value">56 min (principal)</div>
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
                    <a href="https://docs.google.com/document/d/1mdYnniBG5vg4HjMMqqojEs8siFXoRnxi0RfxursBw7A/edit?usp=sharing" class="meta-link">Google Docs</a>
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
    <a href="https://docs.google.com/document/d/1izDWZKR_xB2qj2a8LkbqcnqnjBIC-C7fn-74CIA-m9w/edit?usp=sharing" class="action-button">
        <i class="fas fa-users"></i>
        <span>Contribuer</span>
    </a>
</div>

# Vue d'ensemble

Actuellement, nous peinons à comprendre le fonctionnement des modèles d'IA. Nous savons comment les entraîner et les construire, ce qui signifie que nous pouvons les concevoir et leur apprendre à effectuer des tâches, comme reconnaître des objets dans des images ou générer du texte cohérent en réponse à des invites. Cependant, cela ne signifie pas que nous pouvons toujours expliquer leur comportement après l'entraînement. Pour l'instant, nous ne pouvons pas expliquer pourquoi un réseau a pris une décision spécifique ou produit une sortie particulière. **L'objectif de l'interprétabilité est de comprendre le fonctionnement interne de ces réseaux et d'expliquer comment ils fonctionnent**, ce qui pourrait nous permettre de mieux faire confiance et de contrôler les modèles d'IA.

!!! warning "Avant de lire ce chapitre, il est recommandé de bien connaître les architectures des transformers et des CNN."

<figure class="video-figure" markdown="span">
<iframe style="width: 100%; aspect-ratio: 16 / 9;" frameborder="0" allowfullscreen src="https://www.youtube.com/embed/KuXjwB4LzSA"></iframe>
  <figcaption markdown="1"><b>Vidéo 9.1 :</b> Vidéo facultative. Si vous n'êtes pas familier avec les réseaux de neurones convolutifs (CNN, de l'anglais *Convolutional Neural Networks*), cette vidéo vous aidera à vous mettre à niveau avant de lire ce chapitre.</figcaption>
</figure>

<figure class="video-figure" markdown="span">
<iframe style="width: 100%; aspect-ratio: 16 / 9;" frameborder="0" allowfullscreen src="https://www.youtube.com/embed/aircAruvnKk"></iframe>
  <figcaption markdown="1"><b>Vidéo 9.2 :</b> Vidéo facultative. Si vous n'êtes pas familier avec les transformers, les vidéos sur les transformers dans cette playlist vous aideront à vous mettre à niveau avant de lire ce chapitre.</figcaption>
</figure>

Pour chaque méthode présentée dans ce chapitre, nous fournissons d'abord un aperçu général, suivi d'une explication plus approfondie et technique. Les explications techniques peuvent être sautées.

<div class="section-end">
    <span>❧</span>
</div>