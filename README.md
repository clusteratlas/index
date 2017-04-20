# An open index for HTML5 indie game developers.

- Always open for PR's for contributions :)

## Table Of Contents

- Networking
  - [Networking Basics](#networking-basics)
  - [Networking Libraries](#networking-libraries)
    - [Socket.IO](#socketio)
    - Faye & Faye-Websocket
    - UWS, Engine.io, etc.
- Miscellaneous
  - Learning Javascript
  - [Recommended Reads](#recommended-reads)

---

## Networking Basics

Things that matter: 
- Knowing difference between tcp/udp
- Lightweight vs Feature-rich libraries
- Platform compatibility (ie, can the nodejs server handle connections from browser-based & native-code clients?)
- Being able to do the math for the bandwidth requirements (ie: how many mbps/player can the server handle)
- Being able to do the same math when scaling the server (when using load balancers and multiple server instances and such)
- Being able to use dns-level traffic managers to decrease latency for players in various regions
- Knowing which game data can be fired-and-forget across udp, and which of those should really go over tcp
- Game state restoration on player's side in reconnection
- Implementations really vary by genre, be it arcade/turn-based/first person shooter/mmorpg's/etc
- Furthermore, I believe that doing some self-education on modern cloud technologies (ie Azure/AWS/Google Cloud Platform) would expose you to higher-level scaling & handling of game networking problems from a server-administrator point of view (instead of an indie game developer pov)
- Related reads:
  - http://gafferongames.com/networking-for-game-programmers/
  - https://developer.valvesoftware.com/wiki/Source_Multiplayer_Networking
  - https://0fps.net/2014/02/10/replication-in-networked-games-overview-part-1/
  - https://0fps.net/2014/02/17/replication-in-networked-games-latency-part-2/
  - https://0fps.net/2014/02/26/replication-in-networked-games-spacetime-consistency-part-3/
  - https://0fps.net/2014/03/09/replication-in-network-games-bandwidth-part-4/

## Networking Libraries

### SocketIO
- Features:
  - Simple pub/sub messaging
  - Automatic reconnection
- Notes:
  - Automatic reconnection is quite sketchy especially on the server-side of things.
  
[![website](https://img.shields.io/badge/website-socket.io-blue.svg?style=flat-square)](https://socket.io/)

[![API](https://img.shields.io/badge/API-Server-pink.svg?style=flat-square)](https://github.com/socketio/socket.io/blob/master/docs/API.md)
[![API](https://img.shields.io/badge/API-Client-pink.svg?style=flat-square)](https://github.com/socketio/socket.io-client/blob/master/docs/API.md)

[![npm](https://img.shields.io/badge/npm-socket.io-red.svg?style=flat-square)](https://www.npmjs.com/package/socket.io)
[![npm](https://img.shields.io/badge/npm-socket.io--client-red.svg?style=flat-square)](https://www.npmjs.com/package/socket.io-client)

### Faye & Faye-Websocket

- Features
  - Simple pub/sub messaging
  - Sending of string / buffer
- Notes
  - Biggest advantage over socket.io is its simplicity, flexibility & overall the whole project is notably well-maintained.
  - However automatic reconnection isn't built-in on this one.

[![website](https://img.shields.io/badge/website-faye.jcoglan.com-blue.svg?style=flat-square)](https://faye.jcoglan.com/)

[![github](https://img.shields.io/badge/github-faye-brightgreen.svg?style=flat-square)](https://github.com/faye/faye)
[![github](https://img.shields.io/badge/github-faye--websocket--node-brightgreen.svg?style=flat-square)](https://github.com/faye/faye-websocket-node)

[![npm](https://img.shields.io/badge/npm-faye-red.svg?style=flat-square)](https://www.npmjs.com/package/faye)
[![npm](https://img.shields.io/badge/npm-faye--websocket-red.svg?style=flat-square)](https://www.npmjs.com/package/faye-websocket)

---


## Recommended Reads

- https://www.reddit.com/r/gamedev/comments/66bwxe/7_of_my_worst_gamekilling_assumptions_and_what/

---

- https://nodejs.org/api/
- https://github.com/mscdex/ssh2
- https://www.npmjs.com/package/node-forge
- https://github.com/pierrec/js-xxhash
- https://github.com/Mostafa-Samir/zip-local

- https://www.npmjs.com/package/nodejs-fs-utils
- https://www.npmjs.com/package/pretty-bytes
- https://www.npmjs.com/package/uuid-random
- https://www.npmjs.com/package/chalk
- https://www.npmjs.com/package/eventemitter3

- https://www.npmjs.com/package/xo
- https://www.npmjs.com/package/ava

- https://www.npmjs.com/package/faye-websocket
- https://www.npmjs.com/package/clipboardy
- https://www.npmjs.com/package/globby
- https://www.npmjs.com/package/hasha
- https://www.npmjs.com/package/lodash - https://lodash.com/docs/
- https://www.npmjs.com/package/chokidar
- https://www.npmjs.com/package/yargs - http://yargs.js.org/docs/
- https://www.npmjs.com/package/async - http://caolan.github.io/async/docs.html

- https://www.npmjs.com/package/gulp - http://gulpjs.com/

```sh
npm install gulp-cli -g
npm install gulp -D
```

- https://github.com/webtorrent/webtorrent
- https://github.com/feross/p2p-graph

mongodb:
- https://www.npmjs.com/package/mongodb
- http://mongodb.github.io/node-mongodb-native/2.2/tutorials/crud/

azure storage:
- https://www.npmjs.com/package/azure-storage
- http://azure.github.io/azure-storage-node/


- https://github.com/primus/ejson
- https://github.com/hubspot/vex
- https://github.com/dmauro/Keypress
- http://hammerjs.github.io/
- https://jquery.com/download/
- https://github.com/jriecken/sat-js
- https://github.com/jcubic/jquery.terminal

- https://github.com/lpinca/stopcock
- https://github.com/janhuenermann/neurojs
- https://github.com/sindresorhus/multimatch

Free SSL:
- https://www.sslforfree.com/
- https://www.freessl.com/freessl/good-karma/

- https://github.com/Valve/fingerprintjs2
- https://github.com/dmester/jdenticon
- https://github.com/lafeber/world-flags-sprite

- https://www.npmjs.com/package/highland
> https://gist.github.com/kharandziuk/e823707bf71fba9a4cdf944216773f58
> http://blog.vullum.io/javascript-flow-callback-hell-vs-async-vs-highland/

- https://github.com/winstonjs/winston
