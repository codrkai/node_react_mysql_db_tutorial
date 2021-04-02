# Using MySQL with Node and React JS

This tutorial uses the same project files from node_react_mongodb_tutorial, and modified to use with MySQL database instead of MongoDB.

First, install MYSQL using homebrew

For my case since I'm running MacOS Mojave on my Macbook Pro, I'm going to install MySQL version 5.7
```javascript
brew install mysql@5.7
```

I need to force my MacOS to use MySQL version 5.7
```javascript
brew link --force mysql@5.7
```

(optional) Set up a database password if you would like...
```javascript
mysql_secure_installation
```

Start up the MySQL server
```javascript
brew services start mysql@5.7
```

Other useful commands:
```javascript
brew services restart mysql@5.7
brew services list
brew services cleanup
```

Install MySQL as a package dependency inside of the backend folder
```javascript
cd backend
npm install mysql
```

Install MySQL Workbench
```javascript
For my MacOS Mojave, I installed Workbench version 8.0.18
```

MySQL Workbench:
- Create a Connection
- Create a new Schema (node_twitterclone)
- Create tables (users, tweets)
