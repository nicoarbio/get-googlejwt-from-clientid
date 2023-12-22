# Utilitario para obtener token JWT de google a partir de Google Client ID

> https://nicoarbio.github.io/get-googlejwt-from-clientid/

## Configuración

### Configuración de uso desde Github Page
1. Ir a la consola de Google y agregar `https://nicoarbio.github.io` a los "Orígenes autorizados de JavaScript"

### Configuración de uso desde entorno local (con VSCode)
1. Clonar repo
1. Instalar extensión VSCode
    1. La página si es abierta como un archivo `.html` no funcionará, necesitamos instalar una extensión en VSCode para poder levantar un server local de forma que se pueda acceder a, por ejemplo: `http://localhost:3000/index.html`.
        1. Puede ser cualquier extensión pero recomiendo usar "Five Server" (En marketplace de VSCode con id `yandeu.five-server`).
        1. Una vez instalada configurar dos atributos:
            1. `Host: Set the server host. string`: localhost
            1. `Port: Set the server port. number. usually between 3000 and 9999`: puerto, en este caso 3000.
1. Ir a la consola de Google y agregar `http://localhost:3000` a los "Orígenes autorizados de JavaScript"
1. En VSCode, en la esquina inferior derecha, clickear el botón `Go Live`.
1. En instantes se abrirá en el navegador la página cargada en la url `http://localhost:3000/index.html`.

## Uso
> Importante: Si se detecta el queryParam `clientId`, se inicializará automáticamente el botón, y solo deberás iniciar sesión.
1. Ingresar Google Client ID en el textbox.
1. Inicializar el inicio de sesión mediante el botón "Initialize Google Login with Google Client ID" (El `clientId` se agregará a la url)
1. Iniciar sesión en Google como en cualquier aplicación.
1. Finalmente se podrá ver la información del usuario authenticado.
1. Se puede copiar al portapapeles gracias al botón "Copy to clipboard".
