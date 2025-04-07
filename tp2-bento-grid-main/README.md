# Frontend Mentor - Solution Grille Bento

Il s'agit d'une solution pour le [défi Grille Bento sur Frontend Mentor](https://www.frontendmentor.io/challenges/bento-grid-RMydElrlOj). Les défis de Frontend Mentor vous aident à améliorer vos compétences en codage en construisant des projets réalistes.

## Table des matières

- [Frontend Mentor - Solution Grille Bento](#frontend-mentor---solution-grille-bento)
  - [Table des matières](#table-des-matières)
  - [Aperçu](#aperçu)
    - [Le défi](#le-défi)
    - [Capture d'écran](#capture-décran)
    - [Liens](#liens)
  - [Mon processus](#mon-processus)
    - [Technologies utilisées](#technologies-utilisées)
    - [Ce que j'ai appris](#ce-que-jai-appris)
    - [Développement continu](#développement-continu)
    - [Ressources utiles](#ressources-utiles)
  - [Auteur](#auteur)
  - [Remerciements](#remerciements)


## Aperçu

### Le défi

Les utilisateurs doivent être capables de :

- Voir la mise en page optimale de l'interface en fonction de la taille de l'écran de leur appareil.

### Capture d'écran

![](assets/images/site.png)

### Liens

- URL de la solution : [Ajoutez l'URL de la solution ici](https://github.com/BouMas2231020/tp2-bento-grid-main-Masten)


## Mon processus

### Technologies utilisées

- Marquage HTML5 sémantique
- Propriétés CSS personnalisées
- CSS Grid
- Workflow mobile-first 


### Ce que j'ai appris



```css
.bento-grid-container {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    grid-template-rows: 13rem 13rem 13rem;
    grid-template-areas: 
        'column1 column2 column3'
        'column1 column2 column3'
        'column1 column4 column4'
    ;
    gap: 1rem;
    max-width: 60rem;
    margin-inline: auto;
}

@media screen and (max-width: 950px) {
    .bento-grid-container {
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 13rem 13rem 13rem 13rem;
        grid-template-areas: 
            'column2 column3'
            'column2 column3'
            'column4 column4'
            'column1 column1'
        ;
    }

}

@media screen and (max-width: 650px) {
    .bento-grid-container {
        grid-template-columns: 1fr;
        grid-template-rows: auto auto;
        gap: 2rem;
        grid-template-areas: 
            'column2 '
            'column3 '
            'column4 '
            'column1 '
        ;
    }

}

```

je suis fier de ce css, car je pense que c'est la partie la plus importante de ma compréhension du display: grid. le grid-template-columns: 1fr 2fr 1fr; permet d'avoir une premiere colonne qui occupe 1\4 de l'espace, un deuxieme colonne qui occupe 2\4 de l'espace et une derniere colonne qui occupe 1/4 de l'espace. et le grid-template-rows: 13rem 13rem 13rem; qui definie la taille des rangees et pour moi le plus important cette partie : 

grid-template-areas: 
        'column1 column2 column3'
        'column1 column2 column3'
        'column1 column4 column4'
    ;

Elle permet une grande fléxibilité de la dispostion des element comme dans l'exemple ou les rangees sont définies par les chaines de caractere a l'horizontale et les colonne par l'odre dans lequel a été écrit la chaine de caractère.



### Développement continu

comme dans le tp1 je pense que je devrais continuer à essayer d'améliorer mon organisation surtout dans le css. Je pense aussi que le display: grid; est un outil très puissant pour disposer les éléments qui peut être aussi utliser avec les flexbox donc je vais surement utiliser ces outils dans mes futurs projet.

### Ressources utiles

- [Exemple de ressource 1](https://www.youtube.com/watch?v=OzAc3eC6WQg&ab_channel=KimDoesCode) - Cela m'a aidé pour faire le projet. grace a cette vidéo j'ai vraiment compris le concept de grille et à qu'elle point peut etre utile dans les designs complexe.

## Auteur

- Auteur - [Masten Bournane]
- Frontend Mentor - [BouMas2231020](https://github.com/BouMas2231020/tp2-bento-grid-main-Masten) 

## Remerciements

Comme je l'ai dis auparavant c'est la video KimDoesCode qui m'a aidé a réaliser ce projet.