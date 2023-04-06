# MongoDB-Notes <br/>

### Start MongoDB service on Mac :<br/>
**On default port (27017) :**<br/>
~/mongodb/bin/mongod --dbpath=data/db <br/><br/>

**On specified port :**<br/>
~/mongodb/bin/mongod --dbpath=data/db2 --port 27018 <br/><br/>

### To use MongoDB Tools on Mac :<br/>
**Add to Path variable :**<br/>
export PATH=/Users/kritikushwaha/Downloads/mongodb-database-tools-macos-x86_64-100.5.4/bin:$PATH <br/><br/>

**Go to the directory where tools are saved :**<br/>
cd /Users/kritikushwaha/Downloads/mongodb-database-tools-macos-x86_64-100.5.4/bin <br/><br/>

**Use the import/restore/export/dump commands :**<br/>
mongoimport --uri "mongodb://localhost:27018" --db=test_db --collection=test_events --legacy --file="/Users/kritikushwaha/Desktop/test_events.json"<br/><br/>

mongorestore --gzip --db=test_db --collection=test_events /Users/kritikushwaha/Desktop/test_db/test_events.bson.gz<br/>

