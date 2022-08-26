# Desafio Mocks y Normalizacion - eCommerce Backend #

## _Autor: Rodolfo Gonzalez - Curso: Backend_

- Se presenta desde la ruta ‘/api/productos-test’ del servidor una lista con 5 productos generados al azar utilizando Faker.js como generador de información aleatoria de test.

http://localhost:9090/api/productos-test


- Se reformo el formato de los mensajes y la forma de comunicación del chat, bajo la siguiente estructura:

```
{
    "id": 1,
    "timestamp": "24/8/2022 23:26:37",
    "autor": {
      "email":  "test2@test.com",
      "nombre": "test2",
      "apellido": "test2",
      "edad": 33,
      "alias": "test2",
      "avatar": "https://image.api.playstation.com/vulcan/ap/rnd/202106/3002/Eaq9uyUlyLZK8L5xTlsPl0rM.png"
    },
    "text": "Hola, Como estas?"
  }
```

- Las rutas para obtener todos los mensajes se hace mediante un get a la ruta:
```

http://localhost:9090/api/mensajes
```

- Las rutas para obtener los mensajes por id se hace mediante un get a la ruta:
```
http://localhost:9090/api/mensajes/id
```

- El array que se devuelve esta normalizado con normalizr, conteniendo una entidad de autores, en la siguiente ruta:

```
http://localhost:9090/api/mensajes-normalizados
```

# Para su prueba se puede realizar con Postman

# Para su prueba en front:
1.	Clonar el repositorio ( git clone https://github.com/rodolfogonzalezled/mocks-normalizacion.git)
2.	Obtener node_modules ( npm install )
    - Para la vista se aplico el motor de plantilla EJS (npm install ejs)
    - Se instala los modulos via npm:
        - npm init -y
        - npm install express
        - npm install faker@5.5.3
        - npm i normalizr
3.	Iniciar la app desde la terminal en la carpeta del proyecto a revisar. ( node server.js )
4.	El proyecto se ejecutará en el navegador en ( http://localhost:9090 )  

# Vistas:
- Formulario para cargar un producto, listar productos y centro de mensajes.

##### Proyecto en desarrollo ######
