**commands**:

```
eslint --init
```

Example **.eslintrc **use by [create-react-app](https://github.com/facebook/create-react-app)

```javascript
{
    "extends": "eslint:recommended",
    "env": {
      "browser": true,
      "commonjs": true,
      "node": true,
      "es6": true
    },
    "parser": "babel-eslint",
    "parserOptions": {
      "ecmaVersion": 6,
      "ecmaFeatures": {
          "jsx": true
      }

    },
    "plugins": [
      "react"
    ],
    "rules": {
      "no-console": "off",
      "strict": ["error", "global"],
      "curly": "off",
      "react/jsx-uses-vars": 1

    }
  }
```

Notes:

The plugins section is important, it allows us to use `react/jsx-uses-vars`rule that will prevent `no-unused-vars` warning.

**Install globally**

**`npm i -g eslint babel-eslint eslint-plugin-react`**

