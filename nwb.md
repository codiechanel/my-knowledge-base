You can use NWB to launch a single react file without worrying about dependencies. Perfect for rapid prototyping.

`nwb react run app.js`

**New React App**

`nwb new react-app my-app`

You may not want to use yarn when you use NWB because it will refresh your node modules folder.

If you want to use a proxy, you can add this to config.

```javascript
  devServer : {
    "proxy": {
      "/.netlify/functions": {
        "target": "http://localhost:9000",
        "pathRewrite": {
          "^/\\.netlify/functions": ""
        }
      }
    }
  }
```
