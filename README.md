# _Curso de GIT y GITHUB_

> Inicio: 21/03/2023

## _RAMAS_

:::

    # crear rama
    git branch nombre-rama

    # cambiar de rama
    git checkout nombre-rama

    # crear una rama y cambiarte a ella
    git checkout -b rama

    # eliminar rama
    git branch -d nombre-rama

    # eliminar ramas remotas
    git push origin --delete nombre-rama

    #eliminar rama (forzado)
    git branch -D nombre-rama

    # listar todas las ramas del repositorio
    git branch

    # lista ramas no fusionadas a la rama actual
    git branch --no-merged

    # lista ramas fusionadas a la rama actual
    git branch --merged

    # rebasar ramas
    git checkout rama-secundaria
    git rebase rama-principal

# Fusiones

Une dos ramas. Para hacer una fusión necesitamos:

1. Situarnos en la rama que se quedará con el contenido fusionado.
1. Fusionar.
   
Cuando se fusionan ramas se pueden dar 2 resultados diferentes:

    Fast-Forward: La fusión se hace automática, no hay conflictos por resolver.

    Manual Merge: La fusión hay que hacerla manual, para resolver conflictos de duplicación de contenido.

- nos cambiamos a la rama principal que quedará de la fusión
  
:::

    git checkout rama-principal

- ejecutamos el comando merge con la rama secundaria a fusionar
  
:::

    git merge rama-secundaria

## _version 1.0.0_

Esto es un commit par oficializar la version **1.0.0**
