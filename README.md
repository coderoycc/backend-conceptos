# CONCEPTOS BACKEND
## HTTP
* Existen métodos o verbos que nos permiten hacer peticiones al backend (POST - GET - DELETE - PUT - HEAD - PATCH...)
* Cada verbo indica una acción diferente al servidor
* Se pueden hacer peticiones a servidores mediante herramientas como CURL o POSTMAN. 
* Un ejemplo simple es `curl ifconfig.me` que nos devuelve unicamente nuestra IP pública.
* Cabe resaltar que cada peticion tiene un estado, recurso, metodo, version del protocolo, etc. 
* Cada petición puede ser dirigida a cualquier END-POINT como google.com, unitel.bo, api.comidas.io/ensaladas


## SERVIDORES
* Para que nosotros proporcionemos un servicio mediante un END-POINT podemos usar varios lenguejes de programación. 
* Para cada lenguaje de programación existen frameworks que nos facilitan la vida.
* Cada servidor (end-point) debe devolver algun archivo, datos, siempre con un código por ejemplo 200=OK, 404 = NOT FOUND
* Se envia vistas (html) con un motor de vistas, esto depende de cada lenguaje de programación. 
* <a href="github.com/coderoycc/api-node">AQUÍ</a> hay una API con NODEJS simple y minimalista.

## CACHE
* Hace referencia a un programa que almacena copias de las respuestas que envia un servidor, a razón de no volver a enviar nuevamente los datos.
* Ayuda a la eficiencia y tiempo de carga del servicio.
* Aligera la carga del servidor cuando se requieren reutilizar mismos recursos.
* **Almacenar en CACHE archivos estaticos** es posible mantener en cache los archivos estáticos ya que estos no pueden cambiar. Para lograr esto por defecto las peticiones usan una etiqueta E-TAG que guarda los archivos estaticos segun su etiqueta.
* Cuando el ETAG es diferente significa que la información cambió y es necesario hacer una nueva petición y no usar el cache.
* Tambien existe el **maxAge** que permite guardar un archivo durante un tiempo en cache, sin importar si sufrio alguna modificación.

## COOKIES SESIONES
* Las cookies son datos que se almacenan en el navegador y **son enviados al servidor** en cada petición.
* Las sesiones son guardadas en el servidor y no en la parte del cliente (navegador).
  * La ventaja de las sesiones es que se puede guardar mucha información que en las cookies.

## OPERACIONES CRUD
* Cuando tengamos nuestro servicio siempre es necesario hacer ciertas operaciones que se resumen en CRUD
  * Create: para crear nuevos registros a nuestra BD. (insert)
  * Read: nos permite leer registro(s) (select)
  * Update: nos permite actualizar registro(s) (update)
  * Delete: nos permite eliminar registros (delete)

## Bueanas practicas
* MVC - ORM - MODELOS - ESTRUCTURACION
