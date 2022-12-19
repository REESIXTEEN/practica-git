*¿Qué comando utilizaste en el paso 11? ¿Por qué?*
git reset –hard HEAD~1 Con este comando movemos HEAD al commit anterior y con ‘—hard’ se borran los cambios en el working copy.
*¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?*  
Primero git reflog y luego git reset –hard <commit_id> Con el primer comando podemos ver las acciones que hemos ido haciendo y recuperar el id del commit que hemos perdido con el paso anterior, y con el segundo comando podemos mover HEAD a ese commit y recuperar los cambios realizados en él. 
*El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?* 
No se causa ningún conflicto porque no es posible hacer un merge en este caso, ya que los commits de la rama master están ya contenidos en la rama styled.
*El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?*  
Si hay conflictos ya que las dos ramas tienen un commit en el que se modifica las mismas líneas del archivo git-nuestro.md
*El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?*  
No se producen conflictos ya que las líneas del fichero no son distintas entre las dos ramas (en concreto porque el fichero se encuentra vacío en la rama master)
*¿Qué comando o comandos utilizaste en el paso 25?*  
git log --graph
*El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?* 
Si porque la rama title tiene todos los commits de la rama master.
*¿Qué comando o comandos utilizaste en el paso 27?* 
git reset HEAD~1
*¿Qué comando o comandos utilizaste en el paso 28?* 
git checkout git-nuestro.md
*¿Qué comando o comandos utilizaste en el paso 29?* 
git branch -D title
*¿Qué comando o comandos utilizaste en el paso 30?* 
Primero git reflog y luego git reset –hard <commit_merge>
*¿Qué comando o comandos usaste en el paso 32?* 
Primero git reflog y luego git reset –hard <commit_inicial>
*¿Qué comando o comandos usaste en el punto 33?* 
Primero git reflog y luego git reset –hard <commit_final>
