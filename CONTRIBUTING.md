# Contribuir

El repositorio queda abierto para todos los miembros de [devsChile en GitHub](https://github.com/devschile).

En la medida que sea posible todo script *complejo* que se quiera agregar debería ser su propio paquete de npm, ya sea el original o un fork con los cambios en esta organización u otra parte. **Una buena regla es que si tu script tiene dependencias debería ser su propio paquete, sino puede ir en la carpeta de scripts.**

## Pasos:

- Fork a tu cuenta de GitHub y clone este repo en tu local.
- `$ cd ruta/a/berrea`
- `$ npm install` (probablemente sea mejor usar `sudo` a menos que uses nodenv o nvm).
- Si estás usando la carpeta de scripts deja tu código en `berrea/scripts`, sino:

--

- `npm install -g yo generator-hubot` para instalar el generador de hubot.
- `yo hubot:script` en la carpeta correspondiente para crear el template para un script.
- Una vez [publicado el paquete en npm](https://gist.github.com/coolaj86/1318304) agrégalo a `external-scripts.json` y `package.json`.

--

- Para probar tus cambios localmente: `$ bin/hubot` y activarás a berrea. Ahora ya podrás invocarlo junto con sus comandos y los que hayas escrito.
- Para enviar tus cambios a berrea, haz un [_pull request_](https://github.com/rampmasterspa/proinbot/pulls), coméntalo en [Slack devsChile](http://www.devschile.cl) canal [*#berrea-devs*](http://proinchile.slack.com/messages/bot-dev) y será revisado, testeado, linteado y, si pasa los rigurosos análisis, será agregado.
-  Para más información sobre *Hubot* consulta [Hubot Documentation > Scripting](https://hubot.github.com/docs/scripting/).
-  **No olvides documentar tu código**.
