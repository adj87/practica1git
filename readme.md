
# Readme.md					
----------
**¿Qué comando utilizaste en el paso 11? ¿Por qué?** 
 git reset --hard HEAD~1 porque para perder los cambios en el working copy hay que poner --hard
 
 **¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?** 
git reflog, apunté el id y luego lo puse en el comando git reset hard id 

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
no, porque styled contenía los cambios de master

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
si, porque los commits de la rama a fusionar y la rama actual están modificando el git-nuestro.md y git no sabe cual elegir.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
no, porque es fastforward

**¿Qué comando o comandos utilizaste en el paso 25?**
git log --graph

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
Si, porque la rama master no ha añadido ningún commit desde que se creó la rama title y por tanto puede absorber perfectamente los commits de title sin crear conflicto.

**¿Qué comando o comandos utilizaste en el paso 27?**
git reset HEAD~1

**¿Qué comando o comandos utilizaste en el paso 28?**
git checkout -- git.nuestro.md

**¿Qué comando o comandos utilizaste en el paso 29?**
git branch -D  title

**¿Qué comando o comandos utilizaste en el paso 30?**
git reset --hard HEAD@{1}

**-¿Qué comando o comandos usaste en el paso 32?**
git reset --hard HEAD@{17} (17 en mi caso según mi reflog)

**¿Qué comando o comandos usaste en el punto 33?**
Vuelvo otra vez a hacer git reflog y miro donde se encuentra el commit que tiene mi comentario "añado titulo a git-nuestro.md desde title"; el comando queda git reset --hard HEAD@{5} 
