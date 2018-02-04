**Browser Support**

| Chrome | Safari | Firefox | Opera | IE | Android | iOS |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| yep | yep | nope | 15+ | nope | yep | yep |

**Example:**

```css
div::-webkit-scrollbar {
  /* width: 1em; */
  background-color:#394a5e;
}
div::-webkit-scrollbar-track {
  box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
  -webkit-box-shadow: inset 0 0 6px rgba(0,0,0,0.3);
}
div::-webkit-scrollbar-thumb {
  background-color: darkorange;
  outline: 1px solid slategrey;
}
```



