## History Pushstate and Single Page Apps {#history-pushstate-and-single-page-apps}

If you’re developing a single page app and want history pushstate to work so you get clean urls, you’ll want to enable the following rewrite rule:

`/*    /index.html   200`

Although I have managed to make react router work without this, you should try it in case the router doesn't work.

I encountered some problem when I changed this on the manifest:

**"start\_url": "./index.html"**

I changed it to **"start\_url": "./"**, then my router stopped working. But when I applied the redirect I mentioned above, it worked again. 

## Proxying {#proxying}

Just like you can rewrite paths like`/*`to`/index.html`, you can also set up rules to let parts of your site proxy to external services. Let’s say you need to communicate from a Single Page App with an API on[https://api.example.com](https://api.example.com/)that doesn’t support CORS request. The following rule will let you use /api/ from your JavaScript client:

```
/api/*  https://api.example.com/:splat  200
```

Now all requests to /api/… will be proxied through to[https://api.example.com](https://api.example.com/)straight from our CDN servers without an additional connection from the browser. If the API supports standard HTTP caching mechanisms like Etags or Last-Modified headers, the responses will even get cached by CDN nodes.

### Lambda Functions

Netlify offers aws lambda functions. By default these are cors enabled. You can send additional headers on your response to enable cors.

```javascript
   callback(null, {
        statusCode: 200,
        headers: {
          "Access-Control-Allow-Origin": "*",
          "Access-Control-Allow-Headers":
            "Origin, X-Requested-With, Content-Type, Accept"
        },
        body: JSON.stringify(res)
      });
```

**For the old react-scripts version 1**

**create .babelrc**

```javascript
{
    "presets": [
        [
            "env",
            {
                "targets": { "node": "6.10.0" }
            }
        ]
    ]
}
```

Then...

```
install babel-preset-env
```



