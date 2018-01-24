In particular, a request is preflighted if any of the following conditions is true:

If the request uses any of the following methods:

PUT

DELETE

CONNECT

OPTIONS

TRACE

PATCH

[read more](https://developer.mozilla.org/en-US/docs/Web/HTTP/CORS) for details

Some requests don’t trigger a CORS preflight. Those are called “simple requests”

The only allowed methods are:

* [`GET`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/GET)
* [`HEAD`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/HEAD)
* [`POST`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods/POST)

The only allowed values for the[`Content-Type`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Type)header are:

* `application/x-www-form-urlencoded`
* `multipart/form-data`
* `text/plain`



