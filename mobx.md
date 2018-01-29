If you make an observable map. Observer will get triggered when the map itself changes, like when adding. But if you  just change just the property of an item in the map, it is no longer observable. What you should do is to create a copy of that object, modify it, then replace the existing one. 

