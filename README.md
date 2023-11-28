# Flujo de trabajo de GitHub Actions: Instalar Node.js y comprobar versión

Este flujo de trabajo de GitHub Actions se ejecuta cada vez que se realiza un push a tu repositorio. Su objetivo es instalar Node.js en el runner de GitHub Actions y luego verificar la versión de Node.js que se ha instalado.

## Pasos

1. **Checkout**: Este paso utiliza la acción `actions/checkout@v4` para clonar tu repositorio en el runner de GitHub Actions. Esto es necesario para que el runner pueda acceder a tu código.

2. **Instalar Node.js**: Este paso descarga e instala Node.js en el runner. Utiliza el comando `curl` para descargar el script de instalación de Node.js desde el repositorio de NodeSource. Luego, ejecuta el script con `sudo bash -` para instalar Node.js en el runner.

3. **Comprobar versión de Node.js**: Este paso ejecuta el comando `node -v` para imprimir la versión de Node.js que se ha instalado. Esto te permite verificar que la instalación de Node.js se ha realizado correctamente.

## Uso

Para utilizar este flujo de trabajo, debes tener un repositorio en GitHub y hacer un push a él. El flujo de trabajo se ejecutará automáticamente cada vez que se realice un push.

## Contribuir

Si quieres contribuir a este proyecto, puedes hacerlo a través de pull requests. Por favor, asegúrate de seguir las guías de contribución de este repositorio.

