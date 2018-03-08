// angle in radians

`var angleRadians = Math.atan2(p2.y - p1.y, p2.x - p1.x);`

// angle in degrees

`var angleDeg = Math.atan2(p2.y - p1.y, p2.x - p1.x) * 180 / Math.PI`

convert degrees to radians

```javascript
let radians = (degrees) => {
        return degrees * Math.PI / 180;
      };
```

