# Awesome Chrome DevTools with stars

> Awesome tooling and resources in the Chrome DevTools ecosystem

Tools, protocol drivers, trace viewers, and standalone frontends built around Chrome DevTools and the Chrome DevTools Protocol (CDP). Following the [Awesome Manifesto](https://github.com/sindresorhus/awesome/blob/main/awesome.md) ⭐ 516,567 | 🐛 106 | 📅 2026-09-02, we keep this list focused on what's genuinely useful rather than indexing everything in the space.

## Contents

* [Learning](#learning)
* [Tracing & Profiling](#tracing--profiling)
* [Chrome DevTools Protocol](#chrome-devtools-protocol)
* [Using DevTools frontend with other platforms](#using-devtools-frontend-with-other-platforms)
* [DevTools Extensions](#devtools-extensions)
* [Alumni](#alumni)

***

## Learning

* [Chrome Secret Menus](https://github.com/sparkyrider/chrome-secret-menus) ⭐ 80 | 🐛 1 | 🌐 JavaScript | 📅 2026-07-30 - Guide to Chrome's internal `chrome://` pages and diagnostic tools.
* [Front-end Debugging Tools Handbook](https://github.com/lala-hakobyan/front-end-debugging-handbook) ⭐ 61 | 🐛 2 | 📅 2026-06-23 - Practical guide to front-end debugging across DevTools, framework extensions, and IDEs.
* [Dev Tips](https://umaar.com/dev-tips/) - Large collection of tips as animated gifs.
* [DevTools Tips](https://devtoolstips.org/) - Collection of illustrated tips as mini tutorials.
* [Web cheatcodes](https://codepo8.github.io/web-cheatcodes/) - Browser developer tools for non-developers.
* [Dear Console](https://codepo8.github.io/dearconsole) - A collection of snippets to use in the browser console.

***

## Tracing & Profiling

DevTools Performance traces and V8 `.cpuprofile` logs are plain JSON under the hood, and a few standalone viewers do great things with them:

* [speedscope](https://github.com/jlfwong/speedscope) ⭐ 6,769 | 🐛 160 | 🌐 TypeScript | 📅 2026-05-15 - Fast, interactive flamegraph viewer that imports Chrome `.cpuprofile` and timeline traces.
* [Perfetto](https://github.com/google/perfetto) ⭐ 6,616 | 🐛 356 | 🌐 C++ | 📅 2026-10-09 - System profiling and trace analysis suite ([ui.perfetto.dev](https://ui.perfetto.dev/)) with Chromium trace support and SQL trace querying.
* [cpupro](https://github.com/discoveryjs/cpupro) ⭐ 788 | 🐛 8 | 🌐 TypeScript | 📅 2026-10-07 - Deep V8/Chrome `.cpuprofile` analyzer with flamegraphs, call trees, and hot-spot diagnostics.
* [trace.cafe](https://trace.cafe/) - Share and view web performance traces directly in the DevTools Performance panel ([source](https://github.com/paulirish/trace.cafe) ⭐ 142 | 🐛 12 | 🌐 JavaScript | 📅 2026-07-14).

***

## Chrome DevTools Protocol

Pro-tip: flip on Chrome's built-in [Protocol Monitor](https://developer.chrome.com/docs/devtools/protocol-monitor) (`More tools > Protocol monitor`) to watch live CDP traffic and fire off raw commands right in the browser.

* [ChromeDevTools/devtools-protocol](https://github.com/chromedevtools/devtools-protocol) ⭐ 1,569 | 🐛 8 | 🌐 JavaScript | 📅 2026-10-08 - **Canonical location of the protocol JSON**, TypeScript types, and issue tracker for protocol bugs.
* [DevTools Protocol API Docs](https://chromedevtools.github.io/devtools-protocol/) - Browsable UI for exploring the protocol's domains, methods, and events.

### Developing with the protocol

* [chrome-remote-interface Wiki](https://github.com/cyrus-and/chrome-remote-interface/wiki) ⭐ 4,557 | 🐛 12 | 🌐 JavaScript | 📅 2026-02-09 - Handy recipes for common raw-CDP tasks.
* [Chrome Protocol Proxy](https://github.com/wendigo/chrome-protocol-proxy) ⭐ 253 | 🐛 0 | 🌐 Go | 📅 2026-08-25 - Proxy for inspecting and debugging CDP client traffic.

### The big two automation libraries

* [Playwright](https://github.com/microsoft/playwright) ⭐ 97,344 | 🐛 169 | 🌐 TypeScript | 📅 2026-10-09 - Cross-browser automation for Chromium, Firefox, and WebKit across Node.js, Python, .NET, and Java. See also [awesome-playwright](https://github.com/mxschmitt/awesome-playwright) ⭐ 1,589 | 🐛 8 | 📅 2026-10-02.
* [Puppeteer](https://github.com/puppeteer/puppeteer) ⭐ 95,674 | 🐛 267 | 🌐 TypeScript | 📅 2026-10-09 - High-level Node.js API for controlling Chrome over CDP and WebDriver BiDi. See also [awesome-puppeteer](https://github.com/transitive-bullshit/awesome-puppeteer) ⭐ 2,584 | 🐛 27 | 📅 2024-07-19.

### Libraries for driving the protocol (or a layer above)

* Go: [chromedp](https://github.com/chromedp/chromedp) ⭐ 13,301 | 🐛 0 | 🌐 Go | 📅 2026-10-05 - High-level actions and tasks
* Go: [Rod](https://github.com/go-rod/rod) ⭐ 7,124 | 🐛 214 | 🌐 Go | 📅 2026-08-11 - High-level automation and scraping
* JavaScript/Node.js: [chrome-remote-interface](https://github.com/cyrus-and/chrome-remote-interface) ⭐ 4,557 | 🐛 12 | 🌐 JavaScript | 📅 2026-02-09 - Low-level CDP client
* C#/.NET: [Puppeteer Sharp](https://github.com/hardkoded/puppeteer-sharp) ⭐ 3,924 | 🐛 15 | 🌐 C# | 📅 2026-10-09 - Puppeteer port
* Rust: [Rust Headless Chrome](https://github.com/rust-headless-chrome/rust-headless-chrome) ⭐ 2,953 | 🐛 144 | 🌐 Rust | 📅 2026-06-11 - High-level headless Chrome client
* Ruby: [Ferrum](https://github.com/rubycdp/ferrum) ⭐ 2,062 | 🐛 11 | 🌐 Ruby | 📅 2026-10-05 - High-level API to control Chrome
* Python: [Zendriver](https://github.com/cdpdriver/zendriver) ⭐ 1,456 | 🐛 57 | 🌐 Python | 📅 2026-10-02 - Async CDP browser automation
* Rust: [chromiumoxide](https://github.com/mattsse/chromiumoxide) ⭐ 1,402 | 🐛 61 | 🌐 Rust | 📅 2026-04-03 - Async/tokio library with generated types
* Ruby: [Cuprite](https://github.com/rubycdp/cuprite) ⭐ 1,398 | 🐛 33 | 🌐 Ruby | 📅 2026-10-05 - Capybara driver
* Java: [jvppeteer](https://github.com/fanyong920/jvppeteer) ⭐ 805 | 🐛 14 | 🌐 Java | 📅 2026-10-04 - Headless Chrome for Java
* Go: [cdp](https://github.com/mafredri/cdp) ⭐ 796 | 🐛 14 | 🌐 Go | 📅 2025-12-07 - Type-safe bindings for CDP
* Java: [chrome-devtools-java-client](https://github.com/kklisura/chrome-devtools-java-client) ⭐ 239 | 🐛 51 | 🌐 Java | 📅 2024-07-25 - Low-level protocol client
* Python: [ChromeController](https://github.com/fake-name/ChromeController) ⭐ 229 | 🐛 5 | 🌐 Python | 📅 2025-05-25 - High-level browser mgmt
* PHP: [chrome-devtools-protocol](https://github.com/jakubkulhan/chrome-devtools-protocol) ⭐ 184 | 🐛 20 | 🌐 PHP | 📅 2026-10-01 - Client library
* Python: [PyCDP](https://github.com/hyperiongray/python-chrome-devtools-protocol) ⭐ 147 | 🐛 161 | 🌐 Python | 📅 2026-06-03 - Sans-IO wrappers (see also [Trio driver](https://github.com/hyperiongray/trio-chrome-devtools-protocol) ⭐ 72 | 🐛 72 | 🌐 Python | 📅 2026-04-08)
* Clojure: [clj-chrome-devtools](https://github.com/tatut/clj-chrome-devtools) ⭐ 134 | 🐛 4 | 🌐 Clojure | 📅 2024-09-16 - Autogenerated CDP wrapper
* Kotlin: [kdriver](https://github.com/cdpdriver/kdriver) ⭐ 108 | 🐛 7 | 🌐 Kotlin | 📅 2026-08-31 - High-level coroutine-based automation
* Kotlin: [chrome-devtools-kotlin](https://github.com/joffrey-bion/chrome-devtools-kotlin) ⭐ 62 | 🐛 9 | 🌐 Kotlin | 📅 2026-10-06 - Coroutine-based client library
* Clojure: [cuic](https://github.com/milankinen/cuic) ⭐ 38 | 🐛 4 | 🌐 Clojure | 📅 2025-02-11 - High-level UI test automation
* C#/.NET: [dotnet-chrome-protocol](https://github.com/seclerp/dotnet-chrome-protocol) ⭐ 31 | 🐛 8 | 🌐 C# | 📅 2026-09-06 - Runtime library and schema codegen

### Agentic Browser Automation

> We're *extremely* picky with this section. Everyone is wrapping a browser for agents right now—expect any PR adding another MCP server or agent CLI to be closed unless it has real traction and does something novel with CDP under the hood.

* [chrome-devtools-mcp](https://github.com/ChromeDevTools/chrome-devtools-mcp) ⭐ 53,161 | 🐛 218 | 🌐 TypeScript | 📅 2026-10-09 - Official MCP server for Chrome DevTools, which also includes a [CLI](https://github.com/ChromeDevTools/chrome-devtools-mcp/blob/main/skills/chrome-devtools-cli/SKILL.md) ⭐ 53,161 | 🐛 218 | 🌐 TypeScript | 📅 2026-10-09.
* [Webcmd](https://github.com/agentrhq/webcmd) ⭐ 2,677 | 🐛 50 | 🌐 TypeScript | 📅 2026-09-25 - Compiles site navigation into deterministic per-site CLI commands for AI agents.
* [bdg](https://github.com/szymdzum/browser-debugger-cli) ⭐ 170 | 🐛 43 | 🌐 TypeScript | 📅 2026-10-09 - Persistent background CDP session exposing DOM, network, console, and raw protocol methods as shell commands.
* [Lumen](https://github.com/omxyz/lumen) ⭐ 56 | 🐛 15 | 🌐 TypeScript | 📅 2026-03-30 - Vision-first browser agent with self-healing deterministic replay over CDP.

### Browser Adapters

* [devtools-remote-debugger](https://github.com/Nice-PLQ/devtools-remote-debugger) ⭐ 419 | 🐛 8 | 🌐 JavaScript | 📅 2026-08-14 - Debug a webpage remotely via a CDP agent implemented in client-side JS.
* [Inspect](https://inspect.dev/) - Use DevTools against iOS and Android browsers and WebViews. **(closed source)**

## Using DevTools frontend with other platforms

The DevTools UI is a web app speaking CDP over a WebSocket, so you can embed it or point it at Node, Ruby, mobile webviews, or custom runtimes (see `chrome://inspect` for built-in targets).

* [ChromeDevTools/devtools-frontend](https://github.com/ChromeDevTools/devtools-frontend) ⭐ 4,068 | 🐛 124 | 🌐 TypeScript | 📅 2026-10-09 - Canonical source repo for the Chrome DevTools UI (published to npm as [chrome-devtools-frontend](https://www.npmjs.com/package/chrome-devtools-frontend)).
* [Chii](https://github.com/liriliri/chii) ⭐ 2,245 | 🐛 32 | 🌐 JavaScript | 📅 2025-08-17 & [Eruda](https://github.com/liriliri/eruda) ⭐ 21,214 | 🐛 83 | 🌐 JavaScript | 📅 2025-08-01 - Remote debugging server using the real `devtools-frontend` UI (`Chii`, a modern Weinre replacement) and in-page mobile DevTools console (`Eruda`).
* [vscode-js-debug](https://github.com/microsoft/vscode-js-debug) ⭐ 1,982 | 🐛 125 | 🌐 TypeScript | 📅 2026-10-08 - Official DAP-compliant JavaScript and Chrome CDP debugger powering VS Code.
* [ruby/debug](https://github.com/ruby/debug) ⭐ 1,275 | 🐛 95 | 🌐 Ruby | 📅 2026-06-12 - Ruby's official debugger, which supports connecting Chrome DevTools over CDP (`rdbg --open=chrome`).
* [VS Code - Elements for Microsoft Edge](https://github.com/microsoft/vscode-edge-devtools) ⭐ 829 | 🐛 175 | 🌐 TypeScript | 📅 2026-10-02 - Elements and Network panels embedded inside VS Code.
* [Debugging Node.js with Chrome DevTools](https://medium.com/@paul_irish/debugging-node-js-nightlies-with-chrome-devtools-7c4a1b95ae27) - Guide on debugging and profiling Node.js with `node --inspect`.

***

## DevTools Extensions

* [React Developer Tools](https://chromewebstore.google.com/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi) - Inspect React component hierarchies, props, and profiler flamegraphs.
* [Vue.js Developer Tools](https://github.com/vuejs/devtools) ⭐ 2,921 | 🐛 141 | 🌐 TypeScript | 📅 2026-10-09 - Inspect Vue.js components, state, and routing.
* [Angular DevTools](https://chromewebstore.google.com/detail/angular-devtools/ienfalfjdbdpebioblfackkekamfmbnh) - Component tree inspection and change-detection profiling for Angular.
* [Redux Devtools](https://chromewebstore.google.com/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd) - Time-travel debugging and action history for Redux.
* [Ember.js Inspector](https://chromewebstore.google.com/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi) - Inspect Ember.js objects, routes, and data.
* [Web Component DevTools](https://chromewebstore.google.com/detail/web-component-devtools/gdniinfdlmmmjpnhgnkmfpffipenjljo) - Inspect, modify, and observe custom elements and shadow DOM on the page.
* [Clockwork](https://chromewebstore.google.com/detail/clockwork/dmggabnehkmmfmdffgajcflpdjlnoemp?hl=en) - PHP application profiling and request inspection in DevTools.
* [RailsPanel](https://chromewebstore.google.com/detail/railspanel/gjpfobpafnhjhbajcjgccbbdofdckggg?hl=en-US) - Ruby on Rails request and SQL profiling panel.

## Alumni

Old projects, likely not maintained any longer… But still cool.

* [Facebook Stetho](https://github.com/facebook/stetho) ⚠️ Archived - Native Android debugging with Chrome DevTools.
* [ndb](https://github.com/GoogleChromeLabs/ndb) ⚠️ Archived - Improved Node.js debugging experience built on the DevTools frontend.
* [ios-webkit-debug-proxy](https://github.com/google/ios-webkit-debug-proxy) ⭐ 6,203 | 🐛 21 | 🌐 C | 📅 2025-07-02 - Exposes Mobile Safari & UIWebView instances via CDP.
  * [Remote Debug iOS WebKit adapter](https://github.com/RemoteDebug/remotedebug-ios-webkit-adapter) ⚠️ Archived - Builds on `ios-webkit-debug-proxy` and translates WebKit's Remote Debugging Protocol to CDP.
* [PonyDebugger](https://github.com/square/PonyDebugger) ⭐ 5,849 | 🐛 46 | 🌐 Objective-C | 📅 2023-03-18 - Remote network and Core Data debugging for iOS apps via Chrome DevTools.
* [betwixt](https://github.com/kdzwinel/betwixt) ⭐ 4,558 | 🐛 22 | 🌐 JavaScript | 📅 2021-11-23 - System-level network proxy inspected through a standalone DevTools Network panel.
* [VS Code - Debugger for Chrome](https://github.com/Microsoft/vscode-chrome-debug/) ⚠️ Archived - Original Chrome debugger for VS Code (superseded by built-in [vscode-js-debug](https://github.com/microsoft/vscode-js-debug) ⭐ 1,982 | 🐛 125 | 🌐 TypeScript | 📅 2026-10-08, which has a rich CDP/DAP implementation).
* [PuPHPeteer](https://github.com/rialto-php/puphpeteer) ⚠️ Archived - PHP bridge to Node Puppeteer.
* [Insight](https://github.com/3Dparallax/insight/) ⭐ 915 | 🐛 22 | 🌐 JavaScript | 📅 2021-09-30 - WebGL debugging toolkit for Chrome DevTools.
* [Dirac](https://github.com/binaryage/dirac) ⭐ 775 | 🐛 20 | 🌐 Clojure | 📅 2022-08-26 - ClojureScript debugging with a custom DevTools fork.
* Python CDP driver: [pychrome](https://github.com/fate0/pychrome) ⭐ 649 | 🐛 33 | 🌐 Python | 📅 2024-06-17 - Low-level CDP transport handler.
* [IE Diagnostics Adapter](https://github.com/Microsoft/IEDiagnosticsAdapter) ⚠️ Archived - Protocol adapter translating IE 11 to CDP.
* [thetool](https://github.com/sfninja/thetool) ⭐ 223 | 🐛 14 | 🌐 JavaScript | 📅 2023-01-03 - CPU, memory, coverage, and type profiling for Node.js.
* [DevTools Backend](https://github.com/christian-bromann/devtools-backend) ⭐ 148 | 🐛 7 | 🌐 JavaScript | 📅 2022-02-01 - Standalone implementation of the Chrome DevTools backend to debug arbitrary web environments.
* [Remote Debug Gateway](https://github.com/RemoteDebug/remotedebug-gateway) ⭐ 95 | 🐛 2 | 🌐 JavaScript | 📅 2015-11-04 - Connect a debugging client to multiple browsers at once.
  * Multiuser DevTools: [DevTools Remote](https://github.com/auchenberg/devtools-remote) ⭐ 700 | 🐛 7 | 🌐 CSS | 📅 2017-04-10 - Remotely debug someone else's browser.
* [noice-json-rpc](https://github.com/nojvek/noice-json-rpc) ⭐ 46 | 🐛 9 | 🌐 TypeScript | 📅 2020-09-04 - Proxy-based TypeScript/JS library exposing CDP domains directly as an API.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-10-09._
