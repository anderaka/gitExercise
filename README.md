# gitExercise

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?

He utilizado el comando reset --hard HEAD~1 para volver al paso anterior por que tenia que volver un paso atras de ahí el HEAD~1 y l hard
para que borre los cambios en el working directory

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Primero un reflog para identificar el commit al que se pedia volver, despues el comando checkout con el nombre del commit para ir al mismo,
de ahi comando switch -c para crear una nueva rama con ese HEAD y de ahi he vuelto al estado original de la rama styled y de ahi un merge temp.

- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No ha dado ningun conflicto, solo el mensaje Already up to date por que no habia nada que mergear.

- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?

Si causo conflicto por que los archivos estan modificados en diferentes ramas

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No, fue un fast forward.

- ¿Qué comando o comandos utilizaste en el paso 25?
git log --graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Si que se podría, lo ideal es hacer fast forward cuando la rama que mergeas es la que esta ahead.
En este caso title esta por delante (con la head) de master y por eso se podría haber hecho ff sin problemas

- ¿Qué comando o comandos utilizaste en el paso 27?

git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?

git restore git-nuestro.md

- ¿Qué comando o comandos utilizaste en el paso 29?

git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?

git reflog
git reset a0f172e
git add *
git commit -m ""

- ¿Qué comando o comandos usaste en el paso 32?

git reflog
git reset f572615
git add *
git commit -m ""

- ¿Qué comando o comandos usaste en el punto 33?

git reset dc14699
add git-nuestro.md
git commit -m "vuelta al titulo"
