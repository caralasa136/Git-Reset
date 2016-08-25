##Git reset

Cuando se modifica un archivo en stage, los cambios estan unstaged, y para hacer un `commit` de ésos cambios tienes que primero hacer un stage con `git add`, es peligroso utilizar `reset` con una bandera como `--hard` ya que éso eliminará el cambio y lo sacará del directorio de trabajo, en cambio si se usa por ejemplo solo como `git reset` sin banderas solo regresará el cambio hasta el directorio de trabajo. Ahora por ejemplo, `git reset --soft` no modifica el index del archivo ni el árbol sólo resetea la `head` para hacer commit. `git reset --mixed` resetea al index pero no toca el árbol.
+ Aquí dejo una imagen para visualizar la diferencia entre éstos comandos:
![alt text](https://github.com/caralasa136/Git-Reset/blob/master/reset.jpg)
