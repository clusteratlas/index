## An open list of everything nice, curated for HTML5 Indie Game Developers.

> Always open for PR's for contributions :)

## Table Of Contents

- [Basic Concepts](#basic-concepts)
- [HTML5 Game Engines / Frameworks](#html5-game-engines--frameworks)
- [Physics Engines](#physics-engines)
- [Audio Plugins](#audio-plugins)
- [Performance Monitoring](#performance-monitoring)
- [Input Capture](#input-capture)
- [Date & Time Parsing](#date--time-parsing)
- [Game Networking](#game-networking)
  - [Networking Basics](#networking-basics)
  - [Networking Libraries](#networking-libraries)
    - [Socket.IO](#socketio)
    - [Faye & Faye-Websocket](#faye--faye-websocket)
    - UWS, Engine.io, etc.
  - [Other Libraries](#other-libraries)
- [Learning Javascript](#learning-javascript)
- [Interesting Reads](#interesting-reads)
- [Publishing Games](#publishing-games)
- [Monetizing Games](#monetizing-games)
- [Licensing Games](#licensing-games)
- [Recommended Blogs](#recommended-blogs)
- [Recommended Subreddits](#recommended-subreddits)
- [Developer Tools](#developer-tools)
- [Developer Freebies!](#developer-freebies)
---

## Basic Concepts

- Game Genres
  - https://en.wikipedia.org/wiki/List_of_video_game_genres
- Game Input
  - Keyboard & Mouse
  - Screen Touch Gestures, like taps, swipes, pinch, shake
  - Gamepads & Controllers
  - Audio(from Microphone) & Video(from Camera)
- Game Output
  - Screen size, ratio & orientation (portrait / landscape)
  - Resolution of assets depending on the Pixels Per Inch of the device
  - Frames Per Second
  - WebGL / Canvas
  - Music, Sound Effects & Vibrations
- Deployment Platforms
  - Desktop (Windows, Mac, Linux)
  - Smartphones, and Tablets (Android, iOS, Windows Phone, etc.)
  - Desktop Browsers (Chrome, Firefox, Safari, Opera, Internet Explorer & Edge)
  - Consoles, such as Xbox One, Xbox 360, PS3, PS4, PS Vita, Wii U, New 3DS, etc.
- Game Engines
  - https://en.wikipedia.org/wiki/Game_engine
- Web Hosting, Domain Names & Name Servers
  - https://en.wikipedia.org/wiki/Web_hosting_service
- CDN (Cloud Delivery Networks)
  - https://developer.mozilla.org/en-US/docs/Glossary/CDN

## HTML5 Game Engines / Frameworks / Renderers

- Phaser.IO
  - http://phaser.io/
  - https://phaser.io/examples
- PIXI.js
  - http://pixijs.com/
  - https://pixijs.github.io/examples/
- Three.js
  - A JavaScript 3D Library which makes WebGL simpler.
  - https://threejs.org/
  - https://github.com/mrdoob/three.js/
- Babylon.js
  - http://www.babylonjs.com/
- Panda.js
  - http://www.pandajs.net/
  - http://www.pandajs.net/demos/
- Melon.js
  - http://www.melonjs.org/
  - https://melonjs.github.io/melonJS/
- Kiwi.js
  - http://www.kiwijs.org/
  - http://www.kiwijs.org/examples/
- Playground.js
  - http://playgroundjs.com/
  - https://github.com/rezoner/playground

## Physics Engines

- Matter.js
  - A 2D rigid body physics engine for the web
  - http://brm.io/matter-js/
  - http://brm.io/matter-js/demo/
- Box2d.js
  - Port of Box2D to JavaScript using Emscripten
  - https://github.com/kripken/box2d.js/
  - http://kripken.github.io/box2d.js/demo/webgl/box2d.html
- Ammo.js
  - Direct port of the Bullet physics engine to JavaScript using Emscripten
  - https://github.com/kripken/ammo.js
- Physics.js
  - A modular, extendable, and easy-to-use physics engine for javascript.
  - wellcaffeinated.net/PhysicsJS/
  - https://github.com/wellcaffeinated/PhysicsJS
- Cannon.js
  - A lightweight 3D physics engine written in JavaScript. 
  - http://www.cannonjs.org/
  - https://github.com/schteppe/cannon.js
- P2.js
  - JavaScript 2D physics library
  - https://schteppe.github.io/p2.js/
  - https://github.com/schteppe/p2.js
- SAT.js
  - A simple JavaScript library for performing 2D collision detection
  - http://jriecken.github.io/sat-js/
  - https://github.com/jriecken/sat-js

## Audio Plugins

- Howler.js
  - https://github.com/goldfire/howler.js/
  - https://howlerjs.com/
- Pixi-sound.js
  - https://github.com/pixijs/pixi-sound
  - https://pixijs.github.io/pixi-sound/examples/index.html
  
## Performance Monitoring

- Stats.js
  - JavaScript Performance Monitor
  - https://github.com/mrdoob/stats.js
  
## Input Capture

- Keypress.js
  - A robust Javascript library for capturing keyboard input
  - A keyboard input capturing utility in which any key can be a modifier key. 
  - http://dmauro.github.io/Keypress/
  - https://github.com/dmauro/Keypress
- Hammer.js
  - A javascript library for multi-touch gestures
  - http://hammerjs.github.io/
  - https://github.com/hammerjs/hammer.js
  
## Date & Time Parsing

- Moment.js
  - Parse, validate, manipulate, and display dates and times in JavaScript.
  - http://momentjs.com
- MomentTimezone.js
  - Parse and display dates in any timezone.
  - http://momentjs.com/timezone/
  
## Game Networking

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

### Socket.IO
- Features:
  - Simple pub/sub messaging
  - Automatic reconnection
- Notes:
  - Automatic reconnection is quite sketchy especially on the server-side of things.
  
[![website](https://img.shields.io/badge/website-socket.io-blue.svg?style=flat-square)](https://socket.io/)

[![API](https://img.shields.io/badge/API-Server-brightgreen.svg?style=flat-square)](https://github.com/socketio/socket.io/blob/master/docs/API.md)
[![API](https://img.shields.io/badge/API-Client-brightgreen.svg?style=flat-square)](https://github.com/socketio/socket.io-client/blob/master/docs/API.md)

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

## Learning Javascript

- https://developer.mozilla.org/en-US/docs/Web/JavaScript
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Introduction
- https://github.com/getify/You-Dont-Know-JS
- https://addyosmani.com/resources/essentialjsdesignpatterns/book/
- https://gcanti.github.io/2014/09/25/six-reasons-to-define-constructors-with-only-one-argument.html

## Interesting Reads

- [7 Of My Worst Game-Killing Assumptions, And What They Taught Me](https://www.reddit.com/r/gamedev/comments/66bwxe/7_of_my_worst_gamekilling_assumptions_and_what/)
- [XBOX One HTML5 Game Dev](http://www.html5gamedevs.com/topic/29953-xbox-one-html5-game-dev/)

## Publishing Games

- https://developer.mozilla.org/en-US/docs/Games/Publishing_games
- https://developer.mozilla.org/en-US/docs/Games/Publishing_games/Game_distribution
- https://developer.mozilla.org/en-US/docs/Games/Publishing_games/Game_promotion
- https://developer.mozilla.org/en-US/docs/Games/Publishing_games/Game_monetization

## Monetizing Games

- [Why Indie Game Devs Suck at Marketing](https://indiewatch.net/2016/04/26/why-indie-game-developers-suck-at-marketing/)
- [59 Ways To Monetize Your Indie Game](http://gdu.io/blog/monetization/)

## Licensing Games

- http://www.html5gamedevs.com/topic/772-licensing-vs-rev-share-vs-something-else/
- http://www.html5gamedevs.com/topic/11835-want-to-know-about-non-exclusive-license-of-html5-game/

TrueValhalla: 

> When a publisher expresses an interest in any of your games you'll need to determine a suitable price to charge for licensing. The minimum fee I currently accept for a non-exclusive license is $400, the most I ever charged was $950, and the average is approximately $550. While I don't offer exclusive licenses to publishers, I would currently charge between $4000-$5000 for one. Rental fees are normally non-negotiable, but $50-$75 per month is an average rate.

> You can (and should) set different prices for different publishers. Charge large companies more, especially if they're based in Europe. A quick Google search can give you with an idea of how well financed a company is, and where they are situated. Use this information to determine a suitable value for your work. Negotiating a fee requires good judgement. With some experimentation, you'll be able to determine a publisher's range, and charge accordingly.

>HTML5 games are currently worth a lot of money - keep it that way by maintaining high prices for quality content. Sometimes it is worth throwing away a sale in order to protect future business. I could sell my games for $150-$300 per non-exclusive license to some publishers, but for the sake of maintaining the value of HTML5 games I do not. Only accept a fair price, and do not settle for less than what your content is worth.

## Recommended Blogs

- http://gdu.io/blog/
- https://www.truevalhalla.com/blog/

## Recommended Subreddits

- https://www.reddit.com/r/gamedev/
- https://www.reddit.com/r/gameDevClassifieds/
- https://www.reddit.com/r/INAT/
- https://www.reddit.com/r/gamedevscreens/
- https://www.reddit.com/r/gamedesign/
- https://www.reddit.com/r/devblogs/
- https://www.reddit.com/r/iogames/
- https://www.reddit.com/r/IndieDev/
- https://www.reddit.com/r/IndieGaming/
    
## Developer Tools

- Spritesheet Packers
  - https://github.com/amakaseev/sprite-sheet-packer/releases
  - https://www.codeandweb.com/texturepacker
- Editors
  - https://notepad-plus-plus.org/download/
  - https://atom.io/
  - https://www.sublimetext.com/
  - https://www.jetbrains.com/webstorm/
- Creating Mobile Apps
  - https://cordova.apache.org/
  - https://crosswalk-project.org/
  - http://phonegap.com/
- Version Control
  - https://git-scm.com/downloads
  - https://www.sourcetreeapp.com/
- Terminals / CLI's
  - https://hyper.is/
  - http://cmder.net/
- FTP / SFTP
  - https://winscp.net/eng/download.php
- SSH
  - http://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html

## Developer Freebies

- Microsoft Azure w/ $200 Free, for 30 days
  - https://azure.microsoft.com/en-us/free/
- Google Cloud Platform w/ $300 Free, for 1 year
  - https://cloud.google.com/free/
- Amazon Web Services (AWS) Free Tier, for 1 year
  - https://aws.amazon.com/free/
- Free SSL
  - https://www.sslforfree.com/
  - https://www.freessl.com/freessl/good-karma/
- Free Game Assets
  - GFX / GUI / Characters
    - http://www.kenney.nl/
    - https://www.gamedeveloperstudio.com/
  - SFX / Music
    - https://soundcloud.com/parijat-mishra/sets/original-instrumentals
    - http://www.sonniss.com/gameaudiogdc2017/
    - http://www.youtube.com/c/ourmusicbox
- Other Game Asset Sources
  - http://devassets.com/


---

## Queued / To Be Categorized

- Localization http://i18next.com/

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
