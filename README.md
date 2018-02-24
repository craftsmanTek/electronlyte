# electronlyte
electronlyte is Electron in rust. A cross-browser desktop UI that comes in at under 2MB (compare to the standard NodeJS Electron at over 120MB++)
## How it works
This project runs a type-safe, thread-safe, and performant...native Window(s) environment on MS Windows, Linux, and Mac OSX. The application main window is blazing fast, sans hacks, and is pure rust. In the window we inject the most lighweight version of a webview container - WebKit (Cocoa) on Mac OSX, WebKit (GTK) on Linux and MSHTML on Windows. Into the webview we inject your HTML5 / JavaScript application. Voila!
## Writing your HTML5 / JavaScript
If you are looking for performance, it's advisable to look at "no runtime" JS - i.e. prefer a solution like Svelte https://github.com/sveltejs/svelte over e.g. React or Angular; but you're free to choose.
## Writing your rust code
You don't need to write any rust code at all if you don't want to; but you can if you need to. You may, for example want to run a local database, or use sockets, networking services etc., in a separate thread. With rust these will run reliably, and fast. Interopearability with your JavaScript is built-in and bi-directional. You can call rust code from your JS and you can call JS from rust.
## Interop JS-to-rust
Todo - here I'll write up the mechanism for exposing rust so that it can be called from JS.
## Interop rust-to-JS
Todo - here I'll write up the mechanism for exposing JS so that it can be called from rust.
