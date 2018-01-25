The[`sw-precache-webpack-plugin`](https://github.com/goldhand/sw-precache-webpack-plugin)is integrated into production configuration, and it will take care of generating a service worker file that will automatically precache all of your local assets and keep them up to date as you deploy updates. The service worker will use a [cache-first strategy](https://developers.google.com/web/fundamentals/instant-and-offline/offline-cookbook/#cache-falling-back-to-network) for handling all requests for local assets, including the initial HTML, ensuring that your web app is reliably fast, even on a slow or unreliable network.

Service workers are [not currently supported](https://jakearchibald.github.io/isserviceworkerready/) in all web browsers. Service worker registration [won't be attempted](https://github.com/facebook/create-react-app/blob/master/packages/react-scripts/template/src/registerServiceWorker.js) on browsers that lack support.

Example codes

`let cache = await caches.open('my-cache')`

`let req = new Request('/bookmarks10.json')`

`let stored = await caches.match(req)`

`let keys = await cache.keys()`

`await cache.put(req, new Response\(JSON.stringify\(this.bookmarks.values\(\)\)\))`



