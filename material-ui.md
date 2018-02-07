A note about using CSS with Material-UI.

Your external css may not apply to a Material-UI component since, it's using inline styles. Inline styles take precedence.

You can use `!important` if you want to override these inline styles.

```javascript
import Reboot from 'material-ui/Reboot'
```

&lt;Reboot /&gt;

Material UI provides several methods to customize the components. 

1. Using className. You can use regular css or you can use the withStyles function to create a high order component. 
2. Inline style using the style property.
3. Using variations. Material UI provides a variant property that changes the look and behavior of the component.
4. Global theme variation. Using  theme configuration variables via createMuiTheme\(\). This has an advantage because you can add your own custom values here and inject it to the component. You can also use the `overrides` key.

```javascript
const theme = createMuiTheme({
  overrides: {
    MuiButton: {
      // Name of the styleSheet
      root: {
        // Name of the rule
        background: 'linear-gradient(45deg, #FE6B8B 30%, #FF8E53 90%)',
        borderRadius: 3,
        border: 0,
        color: 'white',
        height: 48,
        padding: '0 30px',
        boxShadow: '0 3px 5px 2px rgba(255, 105, 135, .30)',
      },
    },
  },
});
```


