If you are using React, you will soon realize that you may **"need"** to shift to CSS in JS.

Using CSS in JS allows you to dynamically decorate your React components. While there is a convenience when editing a css file, like auto complete support, it limits you in the long run. Your React components is now tied to a specific className, and thus can only be styled once.

Using CSS in JS allows you to separate the style from the component itself, allowing you to change styles at runtime. Features like changing from light mode to dark mode is common nowadays in applications. In development mode, you can have for instance 10 styles that you loaded into memory. If you do this in traditional Css, this means you need to have 10 css files.

And what about sharability? Since the style is separate from the component, other users could easily decorate it with a new style. Compared, with a static className which is tied to the component. If you are using webpack css modules, this className is even random.

If you want to decorate it, sure you can use another css file. But with complex components that have nested child components, how you are going to style the child components?

Since React is actually an `html in js` technology, i think it follows that we should adopt this approach to css as well.

