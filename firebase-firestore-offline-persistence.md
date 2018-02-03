Enable persistence
```javascript
await firebase.firestore().enablePersistence()
this.db = firebase.firestore()
```
Check this flag if you want to know if data came from cache.
```
querySnapshot.metadata.fromCache
```
This only triggers when user is offline

