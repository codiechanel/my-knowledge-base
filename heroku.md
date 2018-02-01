heroku addons:create mongolab

You can access this variable in your Node.js code as process.env.MONGODB\_URI

mongodb.MongoClient.connect\(process.env.MONGODB\_URI, function \(err, database\) 

  

