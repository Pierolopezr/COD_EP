# Merge de la rama `datos`
* Hacemos `checkout` en la rama `main`
* Con click derecho en la rama `datos` seleccionamos la opcion de realizar un merge   
IMAGEN
* Si lo hacemos asi ya se habran "fusionado las 2 ramas"

# Merge de la rama `interface`
* Primero nos damos cueta de que hay un commit con un mensaje raro por lo que hacemos
  un `checkout revision` para saber que se hizo en ese commit.

  ![checkoutRevision.png](../img/checkoutRevision.png)
* una vez verificado que se hizo hacemos un `checkout` a la rama `interface`
* Dentro de la rama click derecho en el commit que qeremos cambiar su mensaje
  seleccionamos la opcion de `Edti Commit Message`

  ![editComitMensajeInterface.png](../img/editComitMensajeInterface.png)

* Le seleccionamos un nombre adecuado, por ejemplo _añadido dialogo con mensaje "Hola Examen!"_

* Ahora nos damos cuenta de que el ultimo commit contiene un error por lo que usaremos `revert commit`
  para no hacer un `merge` a ese error

  ![RevertCommit.png](../img/RevertCommit.png)
* Y despues de eso ya podremos hacer un `checkout` a la main y hacerle `merge` a la rama `interfeace`
  
![MergeAlRvert.png](../img/MergeAlRvert.png)

* Para finalizar, una vez todo este listo creamos un `commit` para marcar la Release 1.0 
* Ve a Git → Push. En la ventana que se abre, marca también la casilla "Push tags"
* Clic en Push
* Ve a tu repositorio en GitHub, haz clic en la pestaña "Releases", luego en "Draft a new release", selecciona la etiqueta v1.0 en "Tag version" y escribe como título Release v1.0.