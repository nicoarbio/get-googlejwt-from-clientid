# Utilitario para obtener token JWT de google a partir de Google Client ID

## Uso desde Github Page


## Uso local

### Consola de Google
Comprobar que en la consola de Google, el origen `http://localhost:<puerto>` esté habilitado. Para este ejemplo, tomaremos el puerto `3000`.

### Instalar extensión VSCode
1. La página si es abierta como un archivo `.html` no funcionará, necesitamos instalar una extensión en VSCode para poder levantar un server local de forma que se pueda acceder a, por ejemplo: `http://localhost:3000/index.html`.
1. Puede ser cualquier extensión pero recomiendo usar "Five Server" (En marketplace de VSCode con id `yandeu.five-server`).
1. Una vez instalada configurar dos atributos:
    1. `Host: Set the server host. string`: localhost
    1. `Port: Set the server port. number. usually between 3000 and 9999`: puerto, en este caso 3000.

### Acceder al .html desde la extensión
1. En VSCode, en la esquina inferior derecha, clickear el botón `Go Live`.
1. En instantes se abrirá en el navegador la página cargad en la url `http://localhost:3000/index.html`.

### Uso
1. Ingresar Google Client ID en el textbox.
1. Inicializar el inicio de sesión mediante el botón "Initialize Google Login with Google Client ID".
1. Iniciar sesión en Google como en cualquier aplicación.
1. Finalmente se podrá ver la información del usuario authenticado.
1. Se puede copiar al portapales gracias al botón "Copy to clipboard".

> En caso de querer mantener, a modo de log, los datos de múltiples intentos de login, comentar la linea 49.

> Consejo: Puede ser de ayuda configurar la variable `defaultClientId` (linea 28 con valor) para que al recargar la página se inicialice automáticamente el login de Google y así agilizar su uso.