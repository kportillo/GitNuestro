#Solución a Práctica del curso de git, gitHub y Sourcetree

**¿Qué comando utilizaste en el paso 11? ¿Por qué?**
*git reset --hard HEAD~1*
Para deshacer un commit utilizamos la instruccion git reset, con HEAD~1 le decimos que queremos ir al commit anterior y con --hard decimos que borre los cambios 
del working copy.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
*git reflog*
*git reset --hard "Id"*
Primero utilizamos *git reflog* para detectar el "Id" del commit que queremos recuperar, luego con *git reset --hard "Id"* nos movemos al "Id" que identificamos y 
con --hard recuperamos nuestros cambios en el working copy.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
No hay conflicto. Presenta el mensaje Already up-to-date. por que la rama styled ya tiene contenido los cambios de la rama master.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
Si hay conflicto. El contenido de git-nuestro en la rama htmlify es diferente al contenido del mismo archivo en styled, hay que solventar el conflicto y decidir que es lo 
correcto para hacer el merge.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
No hay conflicto. Git ve los cambios que tengo en master y ve que style contiene lo de master así que lo que hace es actualizar con Fast-forward el contenido de master.

**¿Qué comando o comandos utilizaste en el paso 25?**
*git log --graph --decorate --pretty=oneline*

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
Si podría ser fast-forward ya que involucran commits de una lista y el puntero master se movería al puntero title, al hacer el *git merge --nn-ff* creamos un nuevo commit que tiene
dos padres y es a este nuevo commit donde se mueve el puntero master.

**¿Qué comando o comandos utilizaste en el paso 27?**
*git reset HEAD~1*

**¿Qué comando o comandos utilizaste en el paso 28?**
*git checkout -- git-nuestro.md*

**¿Qué comando o comandos utilizaste en el paso 29?**
*git branch -D title*

**¿Qué comando o comandos utilizaste en el paso 30?**
*git reflog*
*git checkout 82a9407*
*git checkout -b title*
*git checkout master*
*git merge title*

**¿Qué comando o comandos usaste en el paso 32?**
*git reflog*
*git checkout 2b8ed70*

**¿Qué comando o comandos usaste en el punto 33?**
*git checkout master*
