# WEBHOOKS
El proyecto se trabajó con webhooks, con los cuales se creó una aplicación que es capaz de 
comunicar Github con Discord mediante nuestro servidor.


## Instalación
1. Ejecutar `npm install` para instalar las dependencias
2. Clonar .env.template a .env y configurar las variables de entorno.
3. Ejecutar `npm run dev` para levantar el proyecto en modo desarrollo
4. Ir a github y crear un repo del proyecto, luego en el proyecto ir a `https://github.com/usuario/repo/settings/hooks/new`
4. Abrir terminal de windows y colocar `ngrok http 3000` y copiar la url
5. Regresar a la pagina de Github, pegar la url y agregarle al final /api/github, luego seleccionar application/json en content type. Despues ir a los envirnonments y copiar el SECRET_TOKEN y pegarlo en la pagina de Github. Seleccionar Let me select individual events y chulear solo issues y stars y clic en add webhook.
6. En Discord: Crear un nuevo servidor, clic derecho, server settings, overview, integations, webhooks, create, captain hook,
personalizar al gusto el nombre y el canal, copiar la url y pegarlo en los environments. El ejercicio fue inspirado en `https://www.youtube.com/watch?v=41NOoEz3Tzc`


## Mas info:
https://docs.github.com/en/webhooks/using-webhooks/creating-webhooks
https://www.youtube.com/watch?v=41NOoEz3Tzc
