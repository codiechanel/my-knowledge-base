## History Pushstate and Single Page Apps {#history-pushstate-and-single-page-apps}

If you’re developing a single page app and want history pushstate to work so you get clean urls, you’ll want to enable the following rewrite rule:

`/*    /index.html   200`

Although I have managed to make react router work without this, you should try it in case the router doesn't work. 

For the old react-scripts version 1

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



