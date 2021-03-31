# Projet-nan-01
Projet NAN 01

## Exercice 1

```algo
VARIABLES
  Nbr_mys EST_DU_TYPE NOMBRE
  Coups EST_DU_TYPE NOMBRE
  Saisi EST_DU_TYPE NOMBRE
DEBUT_ALGORITHME
  Nbr_mys PREND_LA_VALEUR ALGOBOX_ALEA_ENT(1,100)
  Coups PREND_LA_VALEUR 1
  AFFICHER "Entrer un nombre entre 1 et 100"
  LIRE Saisi
  TANT_QUE (Saisi!=Nbr_mys) FAIRE
    DEBUT_TANT_QUE
    SI (Saisi>Nbr_mys) ALORS
      DEBUT_SI
      AFFICHER Saisi
      AFFICHER " est trop grand"
      LIRE Saisi
      FIN_SI
      SINON
        DEBUT_SINON
        AFFICHER Saisi
        AFFICHER " est trop petit"
        LIRE Saisi
        FIN_SINON
    Coups PREND_LA_VALEUR Coups+1
    FIN_TANT_QUE
  AFFICHER "Vous avez trouvé : "
  AFFICHER Nbr_mys
  AFFICHER " en "
  AFFICHER Coups
  AFFICHER " coups"
FIN_ALGORITHME
```

## Exercice 2

```algo
FONCTIONS_UTILISEES
  FONCTION Purge(a,b)
VARIABLES
  a EST_DU_TYPE CHAINE
  b EST_DU_TYPE CHAINE
  Resultat EST_DU_TYPE CHAINE
  i EST_DU_TYPE NOMBRE
DEBUT_ALGORITHME
  Resultat PREND_LA_VALEUR ' '
  POUR i ALLANT_DE 1 A len(a)
    DEBUT_POUR
    SI (Mid(a, i, 1) <> b) ALORS
      DEBUT_SI
      Resultat PREND_LA_VALEUR Resultat & Mid(a, i, 1)
      FIN_SI
    FIN_POUR
FIN_ALGORITHME
RENVOYER Resultat
FIN_FONCTION
```

