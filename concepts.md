# index.js

- valida los datos que pasa el usuario
- si la peticion respeta la estructura esperada, le designa esa "petición" al server

# server.js

- recibir la peticion del usuario
- delegar las acciones al controlador
- devolverle al cliente lo que el controlador le retorna

# controller.js

- ejecutar funciones del model en base a lo que me ejecuta el server
- le retorna al server el resultado del model
- la resspuesta del model puede ser exitosa o no, en controller se valida esa respuesta y se le retorna al server la respuesta final. Por ejemplo, en caso de que el model no encuentre un libro en base de datos, este retona, un false, por ende el controller retorna un "No se encuentra en la base de datos."

# model.js

- modificar la base de datos
- retorna los resultados a controller.js
