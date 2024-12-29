
# ⚡🥷 Application dédiée à l'un des maîtres de l'animation japonaise : Yoshiaki Kawajiri

## 1. Description
Cette application est un projet personnel en **HTML/CSS**.
Il s'agit d'une mise en lumière non exhaustive des oeuvres majeures du réalisateur de films d'animation japonais Yoshiaki Kawajiri.
La Home Page catégorise les oeuvres présentées : films principaux, OAV (films distribués uniquement en vidéo), anthologies (ensemble de courts-métrages de plusieurs réalisateurs), séries TV et contenu additionnel (documentaire, interview).
Chaque oeuvre dispose d'une page dédiée, livrant de détails en présentant notamment un trailer vidéo et une affiche d'origine.
Pour plus d'informations sur le travail de Yoshiaki Kawajiri, consulter la [page Wikipedia](https://fr.wikipedia.org/wiki/Yoshiaki_Kawajiri) dédiée au réalisateur.

---

## 2. Fonctionnalités
Des paramètres de **CSS** avancé sont utilisés pour rendre les éléments cliquables dynamiques au survol de la souris de l'utilisateur :

- *Titre*
  
Utilisation de `@font-face`pour un chargement de la police depuis un serveur distant (**URL**).
Utilisation d'un `box-shadow` pour donner un effet "néon" fluide à la titraille, amplifié au passage de la souris

```
h1 {
    font-family: "Blade Runner Movie Font";
    box-shadow: 0px 0px 25px;
    transition: all 300ms;
}

h1:hover {
    box-shadow: 0px 0px 50px;
}
```

- *Images de présentation des oeuvres*
  
Utilisation d'un effet d'agrandissement pour rendre l'élément dynamique

```
.over {
    filter: drop-shadow(10px 10px 5px black);
    transition: all 300ms;
}

.over:hover {
    transform: scale(1.025);
    box-shadow: 0 0 50px black;
}
```

---

## 3. Accès
1. Accédez directement au projet via [ce lien](https://xylo87.github.io/kawajiri/)

2. Clonez ce projet depuis GitHub :
```bash
   git clone https://github.com/Xylo87/kawajiri.git
   cd kawajiri
```
---

## 4. Améliorations possibles
Changement de la structure **HTML** en `table` du contenu principal pour l'utilisation de **Flexbox**.
L'application gagnerait ainsi en fluidité pour ce qui concerne le **Responsive Design**.

---

## 5. Auteur
Projet réalisé par Théo Arbogast (aka Xylo87).
N'hésitez pas à ouvrir une issue ou à me contacter pour toute suggestion ou question.
