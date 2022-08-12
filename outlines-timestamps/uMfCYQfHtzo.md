# 🗣💬 | CODING Q&A | What are Polyfills? How do we protect API keys? AND MORE!
View the video [here](https://www.youtube.com/watch?v=uMfCYQfHtzo)

## Important links

* CanIUse - https://caniuse.com/
* MDN - https://developer.mozilla.org/

## Outline

* [00:00] Stream Start
* [2:32] Hellos
* [12:16] Explaining all of the overlays / commands
* [21:20] Q&A
  * [22:17] jonahjoe: How to address issues related to IE browser as most of the code doesn't work there (ES6 classes etc...)
    * [23:07] Polyfills
      * [23:45] caniuse.com
    * [31:54] Transpilers (Babel...)
    * [33:35] Core-JS (Polyfills)
    * [36:57] CSS AutoPrefixers
      * [38:01] PostCSS
    * [41:37] Creating an `Array.prototype.reduce()` polyfill
      * [1:00:58] MDN's `Array.prototype.reduce()` polyfill
      * [1:05:08] Using the polyfilled reduce
  * [1:13:24] Lucemans: CJ Opinions on https://github.com/CodingGarden/entropychat.app/pull/25 ?
  * [1:18:07] Alca: What's WeakMap good for?
    * [1:19:08] `WeakMap`
    * [1:21:38] `Map`
  * [1:24:03] kevitaka: How would you secure an api without any sort of user login? For example your front end hits a third party api using an api key. Since you can't securely store the api key on the front end, you move that api call to a node backend. But is there a way to prevent others from accessing your api?
    * [1:27:33] Building a simple API to demonstrate that
      * [1:31:53] Trying the Nasa API
      * [1:50:47] Building the express API
      * [2:03:00] Caching
      * [2:06:33] express-rate-limit
      * [2:09:28] express-slow-down
      * [2:14:01] Creating your own API Key
      * [2:20:55] Browser cache
* [2:24:55] End

Contributed by: @MarcHamamji
