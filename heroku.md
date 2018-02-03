heroku addons:create mongolab

You can access this variable in your Node.js code as process.env.MONGODB\_URI

mongodb.MongoClient.connect\(process.env.MONGODB\_URI, function \(err, database\)


```
git init

git add .

git commit -m "My first commit"
```
Once we have a local git, we can now create a new app on heroku.
```
heroku create

git remote -v

git push heroku master
```
Rename
```
heroku apps:rename newname
```

