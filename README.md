# rezogitnuestro

- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
He utilizado un git reset --hard HEAD~1 para que también deshaga los cambios realizados en el working copy. De haber hecho un reset normal se habrían mantenido los cambios realizados de git-nuestro.md
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Primero hice un git reflog para ver el registro de cambios en el repositorio. A continuación me ubique en el paso anterior al reset y con la id del hash utilice el comando git reset –hard idhash para deshacer el ultimo reset.
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
No fue un conflicto propiamente dicho, lo que ocurre es que la rama styled ya contiene todo el recorrido de master, porque styled es una rama lineal de master. Por lo tanto se queda como esta. En todo caso master tendría que absorber a styled con fast-forward.
 
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Hubo un conflicto porque en ambas ramas mergeadas ya había modificado el archivo git-nuestro.md y toca acceder al archivo para decidir que modificación final tendrá.

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No hubo conflicto debido a que styled era un “avance” lineal de master, es decir, un merge fast-forward sin conflictos.

- ¿Qué comando o comandos utilizaste en el paso 25?
Utilice el comando git log --graph

- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
Podría ser fast foward dado anteriormente habíamos mergeado master con styled y styled con htmlify. Por lo tanto, era simplemente un avance lineal.

- ¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1

- ¿Qué comando o comandos utilizaste en el paso 28?
git reset HEAD git-nuestro.md (aunque sea el único archivo, pero quería probar ese comando)


- ¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title

- ¿Qué comando o comandos utilizaste en el paso 30?
Primero git reflog y copiar la id de cuando hice el merge. Luego un git reset –hard <id>
- ¿Qué comando o comandos usaste en el paso 32?
git reflog y git checkout <id> (entendemos que nos movemos sin hacer reset)

- ¿Qué comando o comandos usaste en el punto 33?
git checkout master (entendemos como estado final la rama master con todos los merge y las ramas eliminadas).
