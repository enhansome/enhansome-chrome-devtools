# Awesome Chrome DevTools with stars

> Awesome tooling and resources in the Chrome DevTools ecosystem

## Contents

* [Learning](#learning)
* [DevTools tooling and ecosystem](#devtools-tooling-and-ecosystem)
* [Chrome DevTools Protocol](#chrome-devtools-protocol)
* [Using DevTools frontend with other platforms](#using-devtools-frontend-with-other-platforms)
* [Applications](#applications)
* [DevTools Extensions](#devtools-extensions)
* [Alumni](#alumni)

***

## Learning

* [Chrome Secret Menus](https://github.com/sparkyrider/chrome-secret-menus) ⭐ 74 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-30 - Comprehensive guide to internal pages and diagnostic tools in Chrome.
* [Front-end Debugging Tools Handbook](https://github.com/lala-hakobyan/front-end-debugging-handbook) ⭐ 58 | 🐛 2 | 📅 2026-06-23 - Practical guide to mastering front-end debugging tools, from Chrome DevTools and framework extensions to AI-enhanced IDE debugging.
* [Dev Tips](https://umaar.com/dev-tips/) - Large collection of tips as animated gifs.
* [DevTools Tips](https://devtoolstips.org/) - Collection of illustrated tips as mini tutorials.
* [Can I DevTools?](https://www.canidev.tools/) - Various workflows, documented. Also a weekly tips & tricks [newsletter](https://canidevtools.substack.com/).
* [Web cheatcodes](https://codepo8.github.io/web-cheatcodes/) - Browser developer tools for non-developers.
* [Dear Console](https://codepo8.github.io/dearconsole) - A collection of snippets to use in the browser console.

***

## DevTools tooling and ecosystem

### Object formatting

* [immutable-devtools](https://github.com/andrewdavey/immutable-devtools) ⭐ 671 | 🐛 11 | 🌐 JavaScript | 📅 2019-11-11 - Custom formatter for Immutable-js values.

### Network Inspection

* [betwixt](https://github.com/kdzwinel/betwixt) ⭐ 4,556 | 🐛 22 | 🌐 JavaScript | 📅 2021-11-23 - System level network proxy, providing inspection via Network panel.

### CPU profile

* [cpuprofilify](https://github.com/thlorenz/cpuprofilify) ⭐ 169 | 🐛 3 | 🌐 JavaScript | 📅 2017-04-20 - Converts output of various profiling/sampling tools to the `.cpuprofile` format.
* [call-trace](https://github.com/brendankenny/call-trace) ⭐ 43 | 🐛 2 | 🌐 JavaScript | 📅 2024-03-01 - Can instrument your JS with hooks, and then generate a `.cpuprofile`  of the of the complete (non-sampled) execution. View either time or call counts.
* [Wishbone Python framework](https://wishbone.readthedocs.io/en/latest/misc/profiling.html) - Profiling data can export as `.cpuprofile`.

### Multimedia

* [snapline](https://github.com/pmdartus/snapline) ⭐ 401 | 🐛 1 | 🌐 JavaScript | 📅 2016-03-17 - Converts timeline screenshots to gif.

### Timeline, Tracing & Profiling

* [DevTools Timeline Viewer](https://chromedevtools.github.io/timeline-viewer/) - Share URLs of your timeline recordings.

### Chrome Debugger integration with Editors

* [VS Code - Debugger for Chrome](https://github.com/Microsoft/vscode-chrome-debug/) ⚠️ Archived - Breakpoint debugging in VS Code.
* [VS Code - Elements for Microsoft Edge](https://github.com/microsoft/vscode-edge-devtools) ⭐ 822 | 🐛 1,185 | 🌐 TypeScript | 📅 2026-02-14 - Elements panel inside VS Code.
* [ChromeREPL](https://github.com/acarabott/ChromeREPL) ⭐ 357 | 🐛 3 | 🌐 Python | 📅 2018-06-12 - Within Sublime Text, use the Chrome console.
* [Sublime Web Inspector](http://sokolovstas.github.io/SublimeWebInspector/) - JavaScript Breakpoint debugging right in Sublime Text.
* [WebStorm/JetBrains Chrome Extension](https://www.jetbrains.com/help/webstorm/2017.1/configuring-javascript-debugger-and-jetbrains-chrome-extension.html) - The WebStorm IDE can debug JavaScript, view the DOM tree, and edit HTML, CSS and JS live.

***

## Chrome DevTools Protocol

* [ChromeDevTools/devtools-protocol](https://github.com/chromedevtools/devtools-protocol) ⭐ 1,531 | 🐛 8 | 🌐 TypeScript | 📅 2026-08-14 - **Canonical location of the protocol JSON**. Issue tracker for protocol bugs. TypeScript types.
* [DevTools Protocol API Docs](https://chromedevtools.github.io/devtools-protocol/) - Easy browsable UI for exploring the protocol's domains, methods and events.

### Developing with the protocol

* [chrome-remote-interface Wiki](https://github.com/cyrus-and/chrome-remote-interface/wiki) ⭐ 4,552 | 🐛 12 | 🌐 JavaScript | 📅 2026-02-09 - Many useful recipes.
* [Chrome Protocol Proxy](https://github.com/wendigo/chrome-protocol-proxy) ⭐ 251 | 🐛 1 | 🌐 Go | 📅 2025-01-31 - Tool for debugging clients using devtools protocol.

### The big two automation libraries

* [Puppeteer](https://github.com/GoogleChrome/puppeteer/) ⭐ 95,459 | 🐛 259 | 🌐 TypeScript | 📅 2026-08-13 - Node.js offering a high-level API to control headless Chrome over the DevTools Protocol. See also [awesome-puppeteer](https://github.com/transitive-bullshit/awesome-puppeteer) ⭐ 2,566 | 🐛 25 | 📅 2024-07-19.
* [Playwright](https://github.com/microsoft/playwright) ⭐ 94,495 | 🐛 145 | 🌐 TypeScript | 📅 2026-08-13 - Library to automate Chromium, Firefox and WebKit with a single API. Available for Node.js, Python, .Net, Java. See also [awesome-playwright](https://github.com/mxschmitt/awesome-playwright) ⭐ 1,553 | 🐛 0 | 📅 2026-08-12.

### Libraries for driving the protocol (or a layer above)

* Go: [chromedp](https://github.com/chromedp/chromedp) ⭐ 13,251 | 🐛 177 | 🌐 Go | 📅 2026-07-14 - High-level actions and tasks for driving browsers
* Go: [Rod](https://github.com/go-rod/rod) ⭐ 7,060 | 🐛 209 | 🌐 Go | 📅 2026-08-11
* JavaScript/Node.js: [chrome-remote-interface](https://github.com/cyrus-and/chrome-remote-interface) ⭐ 4,552 | 🐛 12 | 🌐 JavaScript | 📅 2026-02-09
* Python: [pyppeteer](https://github.com/pyppeteer/pyppeteer) ⭐ 3,941 | 🐛 213 | 🌐 Python | 📅 2024-06-29 - Puppeteer port
* C#/.NET: [Puppeteer Sharp](https://github.com/hardkoded/puppeteer-sharp) ⭐ 3,913 | 🐛 15 | 🌐 C# | 📅 2026-08-13 - Puppeteer port
* TypeScript/Node.js: [Taiko](https://github.com/getgauge/taiko/) ⭐ 3,673 | 🐛 49 | 🌐 JavaScript | 📅 2026-08-03
* Ruby: [Ferrum](https://github.com/route/ferrum) ⭐ 2,036 | 🐛 33 | 🌐 Ruby | 📅 2026-08-10 - high-level API to control Chrome in Ruby
* Ruby: [Cuprite](https://github.com/machinio/cuprite) ⭐ 1,397 | 🐛 44 | 🌐 Ruby | 📅 2026-07-09 - Capybara driver
* PHP: [PuPHPeteer](https://github.com/rialto-php/puphpeteer) ⚠️ Archived - PHP bridge to node Puppeteer
* Java: [jvppeteer](https://github.com/fanyong920/jvppeteer) ⭐ 806 | 🐛 13 | 🌐 Java | 📅 2026-07-24  - Headless Chrome For Java
* Go: [cdp](https://github.com/mafredri/cdp) ⭐ 795 | 🐛 14 | 🌐 Go | 📅 2025-12-07
* Go: [godet](https://github.com/raff/godet) ⭐ 399 | 🐛 2 | 🌐 Go | 📅 2026-03-17
* Java: [chrome-devtools-java-client](https://github.com/kklisura/chrome-devtools-java-client) ⭐ 237 | 🐛 51 | 🌐 Java | 📅 2024-07-25
* Python: [ChromeController](https://github.com/fake-name/ChromeController) ⭐ 229 | 🐛 5 | 🌐 Python | 📅 2025-05-25 - high-level browser mgmt
* Go: [gcd](https://github.com/wirepair/gcd) ⭐ 187 | 🐛 2 | 🌐 Go | 📅 2024-10-16
* PHP: [chrome-devtools-protocol](https://github.com/jakubkulhan/chrome-devtools-protocol) ⭐ 185 | 🐛 20 | 🌐 PHP | 📅 2026-08-14 - A PHP client library for the protocol.
* Python: [PyCDP](https://github.com/hyperiongray/python-chrome-devtools-protocol) ⭐ 146 | 🐛 161 | 🌐 Python | 📅 2026-06-03 - Pure-Python, sans-IO wrappers. See also the [Trio CDP driver](https://github.com/hyperiongray/trio-chrome-devtools-protocol) ⭐ 72 | 🐛 72 | 🌐 Python | 📅 2026-04-08
* TypeScript/Node.js: [chrome-debugging-client](https://github.com/TracerBench/chrome-debugging-client) ⭐ 134 | 🐛 24 | 🌐 TypeScript | 📅 2026-04-15
* Clojure: [clj-chrome-devtools](https://github.com/tatut/clj-chrome-devtools) ⭐ 134 | 🐛 4 | 🌐 Clojure | 📅 2024-09-16 - The CDP wrapper API is autogenerated and will be updated when CDP protocol changes.
* Python: [chromewhip](https://github.com/chuckus/chromewhip) ⭐ 121 | 🐛 17 | 🌐 Python | 📅 2023-08-29 - drop-in replacement for the `splash` service
* C#/dotnet: [chrome-dev-tools](https://github.com/BaristaLabs/chrome-dev-tools) ⭐ 81 | 🐛 9 | 🌐 C# | 📅 2023-11-23 - Protocol wrapper generator that can be customized by editing handlebars templates. Includes .Net Core template.
* Kotlin: [chrome-reactive-kotlin](https://github.com/wendigo/chrome-reactive-kotlin) ⭐ 77 | 🐛 3 | 🌐 Kotlin | 📅 2021-11-04 - reactive (rxjava 2.x), low-level client library in Kotlin
* Kotlin: [chrome-devtools-kotlin](https://github.com/joffrey-bion/chrome-devtools-kotlin) ⭐ 61 | 🐛 9 | 🌐 Kotlin | 📅 2026-08-14 - A coroutine-based client library, providing low-level CDP primitives and high-level extensions.
* TypeScript/Node.js: [Lumen](https://github.com/omxyz/lumen) ⭐ 56 | 🐛 15 | 🌐 TypeScript | 📅 2026-03-30 - Vision-first browser agent with self-healing deterministic replay over CDP.
* Clojure: [cuic](https://github.com/milankinen/cuic) ⭐ 38 | 🐛 4 | 🌐 Clojure | 📅 2025-02-11 - Providing a high-level API for UI test automation over the DevTools Protocol.
* C#/.NET: [dotnet-chrome-protocol](https://github.com/seclerp/dotnet-chrome-protocol) ⭐ 31 | 🐛 8 | 🌐 C# | 📅 2026-07-17 - A runtime library and schema code generation tools for Chrome DevTools Protocol support in C#/.NET.
* Rust: [Rust Headless Chrome](https://github.com/atroche/rust-headless-chrome/) ⭐ 28 | 🐛 0 | 📅 2024-03-08
* TypeScript/Node.js: [noice-json-rpc](https://www.npmjs.com/package/noice-json-rpc) - A proxy-based implementation to expose the CDP as its API.

### Browser Adapters

* [devtools-remote-debugger](https://github.com/Nice-PLQ/devtools-remote-debugger) ⭐ 417 | 🐛 8 | 🌐 JavaScript | 📅 2026-08-14 - Use devtools against a webpage; a CDP agent implemeted in client-side JS.
* [Inspect](https://inspect.dev/) - Use devtools against iOS and Android, easily. Browser and Webviews. **(closed source)**

## Using DevTools frontend with other platforms

#### Android

* [Facebook Stetho](https://github.com/facebook/stetho) ⚠️ Archived - Native Android debugging with Chrome DevTools.
* [j2v8-debugger](https://github.com/AlexTrotsenko/j2v8-debugger) ⭐ 92 | 🐛 5 | 🌐 Kotlin | 📅 2025-02-04 - Debugging JavaScript running in [J2V8](https://github.com/eclipsesource/J2V8) ⭐ 2,628 | 🐛 178 | 🌐 Java | 📅 2025-11-14 with Chrome DevTools.

#### ClojureScript

* [Dirac](https://github.com/binaryage/dirac) ⭐ 775 | 🐛 20 | 🌐 Clojure | 📅 2022-08-26 - Debugging of ClojsureScript.

#### iOS

* [PonyDebugger](https://github.com/square/PonyDebugger) ⭐ 5,852 | 🐛 46 | 🌐 Objective-C | 📅 2023-03-18 - Remote network and data debugging iOS apps with Chrome DevTools.

#### Node.js

* [ndb](https://github.com/GoogleChromeLabs/ndb) ⚠️ Archived - An improved Node.js debugging experience with the DevTools Frontend.
* [thetool](https://github.com/sfninja/thetool) ⭐ 224 | 🐛 14 | 🌐 JavaScript | 📅 2023-01-03 - CPU, memory, coverage, type profiling with Node.
* [Debugging Node.js with Chrome DevTools](https://medium.com/@paul_irish/debugging-node-js-nightlies-with-chrome-devtools-7c4a1b95ae27) - Guide on using the full debugging and profiling support in Node v6.3+.
* [chrome-devtools-frontend](https://www.npmjs.com/package/chrome-devtools-frontend) - Mirror of the frontend that ships in Chrome.

#### Ruby

* [ruby/debug](https://github.com/ruby/debug) ⭐ 1,271 | 🐛 94 | 🌐 Ruby | 📅 2026-06-12 - Debugging functionality for Ruby.

***

## Applications

### Browsers

* [BrowserBox](https://github.com/BrowserBox/BrowserBox) ⭐ 3,892 | 🐛 0 | 🌐 Shell | 📅 2026-08-13 - Embed Chrome in a web page, largely powered by DevTools and supporting multiuser browsing, remote DevTools, audio, and documents like `.docx`, `.pdf`, and more.
* [Puppetromium](https://github.com/dosyago/puppetromium) ⭐ 64 | 🐛 1 | 🌐 JavaScript | 📅 2023-07-23 - A proof-of-concept web browser built with Puppeteer, written in Node.js, HTML and CSS, with 0% client-side JavaScript.

### Web Archivers and Indexers

* [dn](https://github.com/dosyago/dn) ⭐ 3,905 | 🐛 2 | 🌐 JavaScript | 📅 2026-08-09 - Archive and index pages you browse for offline viewing and search, implemented using the `Fetch` domain's interceptions, and works with any Chromium-based browser.

***

## DevTools Extensions

### Workflow

* [Vue.js Developer Tools](https://github.com/vuejs/vue-devtools) ⭐ 24,703 | 🐛 513 | 🌐 TypeScript | 📅 2024-09-11 - Inspect Vue.js components and manipulate their data.
* [Insight](https://github.com/3Dparallax/insight/) ⭐ 914 | 🐛 22 | 🌐 JavaScript | 📅 2021-09-30 - A WebGL debugging toolkit which enables more productive WebGL development and more efficient WebGL applications.
* [BEM devtools](https://github.com/escaton/bem-chrome-devtools) ⭐ 47 | 🐛 3 | 🌐 JavaScript | 📅 2017-09-26 - Inspect BEM entities expressed in `i-bem` framework.
* [Clockwork](https://chromewebstore.google.com/detail/clockwork/dmggabnehkmmfmdffgajcflpdjlnoemp?hl=en) - View PHP application profiling data.
* [RailsPanel](https://chromewebstore.google.com/detail/railspanel/gjpfobpafnhjhbajcjgccbbdofdckggg?hl=en-US) - View Ruby on Rails application profiling data.
* [React Developer Tools](https://chromewebstore.google.com/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi) - Inspect the React component hierarchies.
* [Ember.js Inspector](https://chromewebstore.google.com/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi) - Allows you to inspect Ember.js objects in your application.
* [Angular DevTools](https://chromewebstore.google.com/detail/angular-devtools/ienfalfjdbdpebioblfackkekamfmbnh) - Debugging and Profiling for Angular applications.
* [Backbone Debugger](https://chromewebstore.google.com/detail/backbone-debugger/bhljhndlimiafopmmhjlgfpnnchjjbhd) - Inspect a Backbone application's views, models, events, and routes.
* [Redux Devtools](https://chromewebstore.google.com/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd) - Inspect Redux with actions history, undo and replay.
* [Web Component DevTools](https://chromewebstore.google.com/detail/web-component-devtools/gdniinfdlmmmjpnhgnkmfpffipenjljo) - Inspect, modify and observe Web Components on page.

### Themes

* [Material UI Theme](https://chromewebstore.google.com/detail/material-devtools-theme-c/jmefikbdhgocdjeejjnnepgnfkkbpgjo) - Provides various Material Design inspired themes.

### Performance

* [TracerBench](https://github.com/TracerBench/tracerbench) ⭐ 251 | 🐛 24 | 🌐 TypeScript | 📅 2023-04-26 - A controlled performance benchmarking tool for web applications, providing clear, actionable and usable insights into performance deltas.
* [sloth](https://github.com/denar90/sloth) ⭐ 198 | 🐛 3 | 🌐 JavaScript | 📅 2019-05-03 - Chrome extension allows to enable and save CPU and network throttling for selected tabs.

### Automation

* [k6 browser](https://github.com/grafana/xk6-browser) ⚠️ Archived - Browser automation and end-to-end web testing tool that interacts with browsers and collects frontend performance metrics.
* [Puppeteer IDE](https://github.com/gajananpp/puppeteer-ide-extension) ⭐ 243 | 🐛 13 | 🌐 TypeScript | 📅 2023-11-13 - Standalone Puppeteer playground in browser's developer tools.

## Alumni

Old projects, likely not maintained any longer… But still cool.

* [ios-webkit-debug-proxy](https://github.com/google/ios-webkit-debug-proxy) ⭐ 6,193 | 🐛 19 | 🌐 C | 📅 2025-07-02 - Exposes Mobile Safari & UIWebView instances via the CDP.
  * [Remote Debug iOS WebKit adapter](https://github.com/RemoteDebug/remotedebug-ios-webkit-adapter) ⚠️ Archived - Builts upon ios-webkit-debug-proxy and translates WebKit's Remote Debugging Protocol API to the CDP.
* Python CDP driver: [pychrome](https://github.com/fate0/pychrome) ⭐ 648 | 🐛 33 | 🌐 Python | 📅 2024-06-17 - low level CDP transport handler
* [IE Diagnostics Adapter](https://github.com/Microsoft/IEDiagnosticsAdapter) ⚠️ Archived - Protocol adaptor for Microsoft IE 11 to CDP.
* [DevTools Backend](https://github.com/christian-bromann/devtools-backend) ⭐ 150 | 🐛 7 | 🌐 JavaScript | 📅 2022-02-01 - Standalone implementation of the Chrome DevTools backend to debug arbitrary web environments.
* [Remote Debug Gateway](https://github.com/RemoteDebug/remotedebug-gateway) ⭐ 95 | 🐛 2 | 🌐 JavaScript | 📅 2015-11-04 - Allows you to connect a client to multiple browsers at once.
  * Multiuser DevTools: [DevTools Remote](https://github.com/auchenberg/devtools-remote) ⭐ 700 | 🐛 7 | 🌐 CSS | 📅 2017-04-10 - Remotely debug someone else's browser.
* [go-debugger-devtools](https://github.com/allada/go-debugger-devtools) ⭐ 42 | 🐛 0 | 🌐 Go | 📅 2017-07-26

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-14._
