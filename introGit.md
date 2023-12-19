## Introduccion a Git

1. ```git init``` para iniciar el repositorio.
1. ```git status``` muestra el estado actual del repositorio.
1. ```git config -l``` para ver mi configuracion en git.
1. ```git add```  agrega cambios al área de preparación (staging area).
1. ```git commit -m "mensaje"``` confirmar los cambios que has agregado al área de preparación (staging area).
1. ```git log``` muestra el historial de commits de un repositorio.
1. ```git show```  se utiliza en Git para mostrar información detallada sobre un commit específico. Se puede utilizar este comando para ver los cambios introducidos en un commit.
8. ```git diff``` muestra las diferencias entre dos estados. 
9. ```git log --stat``` muestra los cambios especificos en los archivos apartir del commit

---
### Staging repositorio
> Staging es un area temporal antes de enviar los cambios al repositorio.

> es una area en memoria ram, que se encuentra desconectado de todo y se le agregan cambios mediante el comando ```git add```

> el comando ```git commit -m "mensaje"``` se envian los datos de staging al repositorio.

---

## git reset / git checkout

- Que hacer si debo regresar al estado anterior ?
> ```git reset``` permite deshacer cambios en el repositorio. 
> - ```git reset <commitHash> --hard```: todo vuelve al estado anterior.
> - ```git reset <commitHash> --soft```: vuelve al estado anterior, pero lo que se tiene en staging se mantiene.
>
> Tener cuidado con el hard.

> ```git checkout```

---
## Branch

* Cada vez que se realiza un commit, se crea una nueva version.
* Por lo general estamos en la rama **master**.
* Se puede crear ramas para **experimentos/development**.
* ```hotfix``` es una rama especial cuando se tiene un bug en la rama actual/principal, aqui se realiza los cambios y luego se fuciona con la rama actual, realizando un ```merge```.
* ```merge``` cuando se fucionan dos ramas. 
![Alt text](image.png)

