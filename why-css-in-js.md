If you are using React, you will soon realize that you may **"need"** to shift to CSS in JS.

Using CSS in JS allows you to dynamically decorate your React components. While there is a convenience when editing a css file, like auto complete support, it limits you in the long run. Your React components is now tied to a specific className, and thus can only be styled once. 

Using CSS in JS allows you to separate the style from the component itself, allowing you to change styles at runtime. Features like changing from light mode to dark mode is common nowadays in applications. 

And what about sharability? Since the style is separate from the component, other users could easily decorate it with a new style. Compared, with a static className tied to the component. If you are using webpack css modules, this className is even random. 

