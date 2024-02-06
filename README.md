> # Attention, we are undergoing maintenance until 02/08/2024, new documentation and a functional update of the Venom BOT will be available

> # Atenção estámos em manutenção até dia 08/02/2024 estará no ar uma nova documentação e uma atualização funcional do Venom BOT


# 🕷Venom Bot🕸

[![npm version](https://img.shields.io/npm/v/venom-bot.svg?color=green)](https://www.npmjs.com/package/venom-bot)
![node](https://img.shields.io/node/v/venom-bot)
[![Downloads](https://img.shields.io/npm/dm/venom-bot.svg)](https://www.npmjs.com/package/venom-bot)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/orkestral/venom.svg)](http://isitmaintained.com/project/orkestral/venom 'Average time to resolve an issue')
[![Percentage of issues still open](http://isitmaintained.com/badge/open/orkestral/venom.svg)](http://isitmaintained.com/project/orkestral/venom 'Percentage of issues still open')
<a href="https://discord.gg/qCJ95FVbzR"><img src="https://img.shields.io/discord/772885202351292426?color=blueviolet&label=discord&style=flat" /></a>

[![Build Status](https://img.shields.io/github/actions/workflow/status/orkestral/venom/build.yml?branch=master)](https://github.com/orkestral/venom/actions)
[![Lint Status](https://img.shields.io/github/actions/workflow/status/orkestral/venom/lint.yml?branch=master&label=lint)](https://github.com/orkestral/venom/actions)
[![release-it](https://img.shields.io/badge/%F0%9F%93%A6%F0%9F%9A%80-release--it-e10079.svg)](https://github.com/release-it/release-it)

> English: Venom is a high-performance system developed with JavaScript to create a bot for WhatsApp, support for creating any interaction, such as customer service, media sending, sentence recognition based on artificial intelligence and all types of design architecture for WhatsApp.

> Português: Venom é um sistema de alto desempenho desenvolvido em JavaScript para criação de bot para WhatsApp, suporte para criação de qualquer interação, como atendimento ao cliente, envio de mídia, reconhecimento de frases baseado em inteligência artificial e todo tipo de arquitetura de design para WhatsApp.

> Espanõl: Venom es un sistema de alto rendimiento desarrollado con JavaScript para crear un bot para WhatsApp, soporte para crear cualquier interacción, como atención al cliente, envío de medios, reconocimiento de frases basado en inteligencia artificial y todo tipo de arquitectura de diseño para WhatsApp.



## Group of Support - Grupo de Suporte - Grupo de Apoyo
<a target="_blank" href="https://chat.whatsapp.com/Kpm6sPivtQM99vfk9Nnasz" target="_blank"><img title="whatzapp" height="100" width="375" src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f7/WhatsApp_logo.svg/2000px-WhatsApp_logo.svg.png"></a>

## Installation - Instalação - Instalación

```bash
> npm i --save venom-bot
```

English: Installing the current repository "you can download the beta version from the current repository!"

Português: Instalando o repositório atual "você pode baixar a versão beta do repositório atual!"

Espanõl: Instalación del repositorio actual "¡Puedes descargar la versión beta desde el repositorio actual!"

```bash
> npm i github:orkestral/venom
```

## Getting started - Início rápido

```javascript
// Supports ES6
// import { create, Whatsapp } from 'venom-bot';
const venom = require('venom-bot');

venom
  .create({
    session: 'session-name' //name of session
  })
  .then((client) => start(client))
  .catch((erro) => {
    console.log(erro);
  });

function start(client) {
  client.onMessage((message) => {
    if (message.body === 'Hi' && message.isGroupMsg === false) {
      client
        .sendText(message.from, 'Welcome Venom 🕷')
        .then((result) => {
          console.log('Result: ', result); //return object success
        })
        .catch((erro) => {
          console.error('Error when sending: ', erro); //return object error
        });
    }
  });
}
```



## Maintainers - Manutenção - Mantenimiento

English: Maintainers are needed, I cannot keep with all the updates by myself. If you are
interested please open a Pull Request.

Português: São necessários mantenedores, não consigo acompanhar todas as atualizações sozinho. Se você estiver
interessado, por favor abra um Pull Request.

Espanõl: Se necesitan mantenedores, no puedo mantenerme al día con todas las actualizaciones solo. Si usted es
Si está interesado, abra una solicitud de extracción.

## Contributing - Contribuição - Contribución

English: Pull requests are welcome. For major changes, please open an issue first to
discuss what you would like to change.

Português: Solicitações pull são bem-vindas. Para mudanças importantes, abra um problema primeiro para
discuta o que você gostaria de mudar.

Espanõl: Las solicitudes de extracción son bienvenidas. Para cambios importantes, abra primero un problema para
discuta lo que le gustaría cambiar.
