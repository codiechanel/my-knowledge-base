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



