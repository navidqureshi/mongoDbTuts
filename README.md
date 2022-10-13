# Mongodb Commands
## To make a database
```javascript
use databaseName
```

## To insert into a collection | To make a collection
```javascript
db.collectionName.insertOne({key1:value1,....}) // to insert only one record in collection
db.collectionName.insertMany([
    {key1:value1,...}, //record1
    {key1:value1,...}, //record2
    .
    .
    {key1:value1,...} //record n
])
```
## To update one object 
```javascript
db.collectionName.updateOne(
    { _id:ObjectId("//object id number") },
    {
        $set:{
            key1:value1,
            key2:value2,
            .
            .
            keyN:valueN
        }
    }
)
```