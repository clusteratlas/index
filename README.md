## An open list of everything nice, curated for HTML5 Indie Game Developers.

> Always open for PR's for contributions :)

## Table Of Contents

- [Basic Concepts](#basic-concepts)
- [HTML5 Game Engines / Frameworks / Renderers](#html5-game-engines--frameworks--renderers)
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
- [Maps](#maps)
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
- Gameplay, Game Design, Balancing, etc.
  - https://en.wikipedia.org/wiki/Game_design
  - https://en.wikipedia.org/wiki/Gameplay
  - https://en.wikipedia.org/wiki/Game_mechanics
  - https://en.wikipedia.org/wiki/Balance_(game_design)
  - https://en.wikipedia.org/wiki/Dynamic_game_difficulty_balancing

---

## HTML5 Game Engines / Frameworks / Renderers

- Phaser.IO
  - Phaser is a fun, free and fast 2D game framework for making HTML5 games for desktop and mobile web browsers, supporting Canvas and WebGL rendering. 
  - http://phaser.io/
  - https://phaser.io/examples
  - https://github.com/photonstorm/phaser
- PIXI.js
  - Super fast HTML 5 2D rendering engine that uses webGL with canvas fallback
  - http://pixijs.com/
  - https://pixijs.github.io/examples/
  - https://github.com/pixijs/pixi.js
- Three.js
  - A JavaScript 3D Library which makes WebGL simpler.
  - https://threejs.org/
  - https://github.com/mrdoob/three.js/
- WhiteStorm.js
  - Super-fast 3D framework for Web Applications & Games. Based on Three.js
  - https://github.com/WhitestormJS/whitestorm.js
  - https://whs-dev.surge.sh/examples/
- Babylon.js
  - Babylon.js: a complete JavaScript framework for building 3D games with HTML 5 and WebGL 
  - http://www.babylonjs.com/
  - https://github.com/BabylonJS/Babylon.js
- Panda.js
  - Free HTML5 game engine for mobile and desktop with Canvas and WebGL rendering.
  - http://www.pandajs.net/
  - http://www.pandajs.net/demos/
  - https://github.com/ekelokorpi/panda-engine
- Melon.js
  - A fresh & lightweight javascript game engine 
  - http://www.melonjs.org/
  - https://melonjs.github.io/melonJS/
- Kiwi.js
  - Kiwi.js is a blazingly fast mobile & desktop browser based HTML5 game framework. It uses CocoonJS for publishing to the AppStore.
  - http://www.kiwijs.org/
  - http://www.kiwijs.org/examples/
- Playground.js
  - Playground.js is a framework for your javascript based games. It gives you out-of-box access to essentials like mouse, keyboard, sound and well designed architecture that you can expand to your needs.
  - http://playgroundjs.com/
  - https://github.com/rezoner/playground
- Stage.js
  - 2D JavaScript library for cross-platform HTML5 game development 
  - http://piqnt.com/stage.js/
  - https://github.com/shakiba/stage.js
- Cocos2d-x
  - Cocos2d-x is a suite of open-source, cross-platform, game-development tools used by millions of developers all over the world.
  - http://www.cocos2d-x.org/
  - https://github.com/cocos2d/cocos2d-x
- PlayCanvas
  - https://playcanvas.com/
  - https://playcanvas.com/explore
  - https://github.com/playcanvas/engine
- Atomic Game Engine
  - The Atomic Game Engine is a multi-platform 2D and 3D engine with a consistent API in C#, JavaScript, TypeScript, and C++. It deploys natively to Windows, OSX, Android, iOS, and HTML5.
  - https://atomicgameengine.com/
  - https://github.com/AtomicGameEngine/AtomicGameEngine/
- Crafty.js
  - Crafty is a JavaScript game library that can help you create games in a structured way.
  - http://craftyjs.com/
  - https://github.com/craftyjs/Crafty
- Goo.js
  - Goo Engine is an open-source 3D engine using HTML5 and WebGL for rendering.
  - https://github.com/GooTechnologies/goojs
  - https://learn.goocreate.com/
- Create.js
  - A suite of modular libraries and tools which work together or independently to enable rich interactive content on open web technologies via HTML5.
  - http://createjs.com/
  - http://createjs.com/#demos
  - https://github.com/CreateJS
  - Easel.js
    - A JavaScript library that makes working with the HTML5 Canvas element easy. The Easel Javascript library provides a full, hierarchical display list, a core interaction model, and helper classes to make working with the HTML5 Canvas element much easier.
    - http://createjs.com/easeljs
    - https://github.com/CreateJS/EaselJS
  - Tween.js
    - A JavaScript library for tweening and animating HTML5 and JavaScript properties. A simple but powerful tweening / animation library for Javascript. Part of the CreateJS suite of libraries.
    - http://createjs.com/tweenjs
    - https://github.com/CreateJS/TweenJS
  - Sound.js
    - A JavaScript library that lets you easily and efficiently work with audio on the web. A Javascript library for working with Audio. It provides a consistent API for loading and playing audio on different browsers and devices. Currently supports WebAudio, HTML5 Audio, Cordova / PhoneGap, and a Flash fallback.
    - http://createjs.com/soundjs
    - https://github.com/CreateJS/SoundJS
  - Preload.js
    - A JavaScript library that lets you manage and co-ordinate the loading of assets. PreloadJS makes preloading assets & getting aggregate progress events easier in JavaScript. It uses XHR2 when available, and falls back to tag-based loading when not.
    - http://createjs.com/preloadjs
    - https://github.com/CreateJS/PreloadJS

---

## Physics Engines

- Planck.js
  - Planck.js is JavaScript rewrite of Box2D physics engine for cross-platform HTML5 game development.
  - http://piqnt.com/planck.js/
  - https://github.com/shakiba/planck.js
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

---

## Audio Plugins

- Howler.js
  - Javascript audio library for the modern web.
  - https://github.com/goldfire/howler.js/
  - https://howlerjs.com/
- Pixi-sound.js
  - WebAudio API playback without any Flash shims or HTML Audio fallback 
  - https://github.com/pixijs/pixi-sound
  - https://pixijs.github.io/pixi-sound/examples/index.html

---

## Performance Monitoring

- Stats.js
  - JavaScript Performance Monitor
  - https://github.com/mrdoob/stats.js

---

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

---
  
## Date & Time Parsing

- Moment.js
  - Parse, validate, manipulate, and display dates and times in JavaScript.
  - http://momentjs.com
- MomentTimezone.js
  - Parse and display dates in any timezone.
  - http://momentjs.com/timezone/

---

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

## Maps

- Leaflet.js
  - An open-source JavaScript library for mobile-friendly interactive maps.
  - http://leafletjs.com/
  - https://github.com/Leaflet/Leaflet
- OpenLayers
  - A high-performance, feature-packed library for all your mapping needs.
  - https://openlayers.org/
  - https://github.com/openlayers/openlayers

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
    
- [Free Music, Sound Effects and Images for Your Projects by Eric Matyas.](http://www.html5gamedevs.com/topic/27581-building-a-library-of-images-for-everyone/)

```
Hi everyone,

I've been building a library of images that you are welcome to use in your projects. 
They are all original...all my own work. I think a lot of them could be made into 
cool textures for games.  All I ask is to be attributed as indicated on my homepage:

http://soundimage.org/

The images are on my "TXR" pages.  

I'm adding new ones all the time, so be sure to check back often. I sincerely hope that some of them 
are useful. Any and all constructive feedback is welcome and always appreciated.  :-)

All the best,

Eric
```

- [1000 Free Instrumental Game Background Music Tracks](https://www.reddit.com/r/gamedev/comments/66v29j/my_1000_free_instrumental_background_music_tracks/)

```
Torrent (thanks to Aizome) :
https://drive.google.com/open?id=0B3re2AF_gdUhVHlFUDZhQnN4MFU
Soundclick:
http://www.soundclick.com/_mobileFrame.cfm?bandID=1277008
My blog where I release the songs and FLstudio project files for them:
http://anttismusic.blogspot.fi
```

- [500 Male & Female Dialog Pack Audio Files](https://www.reddit.com/r/gamedev/comments/66wzgs/i_just_published_a_free_dialogue_pack_with_over/)

```
[Super Dialogue Audio Pack](https://stuckeast.itch.io/sdap) contains more than 500 audio files of dialogue 
recorded specifically for video games. The pack includes both male and female voices from 5 different voice 
actors, and all of the files can be used for commercial purposes (royalty free).
The pack is available for free at https://stuckeast.itch.io/sdap and a short sample 
can be [heard here](https://soundcloud.com/dillonbecker-1/sdap) (or at the itch.io link).
[Link to full list of lines](https://drive.google.com/file/d/0Byy6MF-H-jRBRzV1X19kbTJKYzA/view) 
and [link to the license](https://drive.google.com/file/d/0Byy6MF-H-jRBa095SEZ6ODV6Ykk/view).
Enjoy!
```

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
