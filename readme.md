- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

**Utilizo git reset --hard HEAD~1 para volver al commit anterior y el modificador --hard para eliminar los cambios en mi working copy**

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

**git reflog para localizar el commit que deshice, y git reset --hard para mover la rama al commit y recuperar los cambios en mi working copy**


- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

**No creó conflictos, htmlify tiene todos los cambios y master no tiene ningún cambio que no tenga htmlify**

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

**Si, causa conflictos, hemos hecho cambios en el mismo archivo en dos ramas diferentes, htmlify no "conoce" el commit que hicimos en matrix**

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

**No creó conflictos, se realizó un merge fast forward (grafo lineal), con lo cuál no existen conflictos, con mover el puntero de master a htmlify es suficiente**

- ¿Qué comando o comandos utilizaste en el paso 25?

**git log --graph --decorate --pretty=oneline**

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

**Si se podría, title contiene todos los cambios, solo es necesario mover el puntero de master a la posición de title**


- ¿Qué comando o comandos utilizaste en el paso 27?

**git reset HEAD~1 para mover el puntero un commit hacía atrás**


- ¿Qué comando o comandos utilizaste en el paso 28?

**git checkout —- poem.md**

- ¿Qué comando o comandos utilizaste en el paso 29?

**git branch -D title**


- ¿Qué comando o comandos utilizaste en el paso 30?

**git reflog para buscar el commit que necesito**
**git checkout 41803ff para mover HEAD al commit donde realicé el cambio**
**git branch title para crear la rama apuntando a ese commit**
**git checkout master y git merge title para mergear con title**


- ¿Qué comando o comandos usaste en el paso 32?

**git reflog para buscar el commit inicial**
**git checkout beecf40**

- ¿Qué comando o comandos usaste en el punto 33?

**git checkout master (apunta al último cambio)**