show dbs

##use collection:
use nameOfcollection

##crud operation:
1)db.nameofdata.insertOne({})
2)db.nameofdata.insertMany({})


##work:
Microsoft Windows [Version 10.0.22631.4317]
(c) Microsoft Corporation. All rights reserved.

C:\Users\sharm>mongosh
Current Mongosh Log ID: 672b50c064292dc1f00d818f
Connecting to:          mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.3
Using MongoDB:          8.0.3
Using Mongosh:          2.3.3

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/

------
   The server generated these startup warnings when booting
   2024-11-06T15:02:45.447+05:30: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test> show dbs
Employes   40.00 KiB
admin      40.00 KiB
config    108.00 KiB
local      40.00 KiB
test> show dbs
Employes   40.00 KiB
admin      40.00 KiB
config    108.00 KiB
local      40.00 KiB
test> show colletions
MongoshInvalidInputError: [COMMON-10001] 'colletions' is not a valid argument for "show".
test> show collections

test> use Mongodb
switched to db Mongodb
Mongodb> show dbs
Employes   40.00 KiB
admin      40.00 KiB
config    108.00 KiB
local      40.00 KiB
Mongodb> db.students.insertOne({name:"Sam", Div:"B"})
{
  acknowledged: true,
  insertedId: ObjectId('672b595e64292dc1f00d8190')
}
Mongodb>
(To exit, press Ctrl+C again or Ctrl+D or type .exit)
Mongodb> mongo
ReferenceError: mongo is not defined
Mongodb>
(To exit, press Ctrl+C again or Ctrl+D or type .exit)
Mongodb>

C:\Users\sharm>mongo
'mongo' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\sharm>mongosh
Current Mongosh Log ID: 672b5996e053edfeb80d818f
Connecting to:          mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.3
Using MongoDB:          8.0.3
Using Mongosh:          2.3.3

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/

------
   The server generated these startup warnings when booting
   2024-11-06T15:02:45.447+05:30: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test> show dbs
Employes   40.00 KiB
Mongodb    40.00 KiB
admin      40.00 KiB
config    108.00 KiB
local      40.00 KiB
test> show collections

test>  Mongodb.students.insertOne(name:"Sam"})
Uncaught:
SyntaxError: Unexpected token, expected "," (1:32)


test> show dbs
Employes   40.00 KiB
Mongodb    40.00 KiB
admin      40.00 KiB
config    108.00 KiB
local      40.00 KiB
test       40.00 KiB
test> use Employes
switched to db Employes
Employes> show collections
Manager
Employes> db.Manager.find()

[
  {
    _id: ObjectId('672b4b587dc47c1281a3f3d7'),
    name: 'DEEPIKA',
    Role: 'SDE'
  }
]
Employes> db.Manager.insertOne({name:"ABS" ,Div:"B"})
{
  acknowledged: true,
  insertedId: ObjectId('672b5bb9e053edfeb80d8191')
}
Employes> db.Manager.find()
[
  {
    _id: ObjectId('672b4b587dc47c1281a3f3d7'),




    ##NEW ADDED###################

 Microsoft Windows [Version 10.0.22631.4317]
(c) Microsoft Corporation. All rights reserved.

C:\Users\sharm>mongosh
Current Mongosh Log ID: 672f1a906fb0511fe80d818f
Connecting to:          mongodb://127.0.0.1:27017/?directConnection=true&serverSelectionTimeoutMS=2000&appName=mongosh+2.3.3
Using MongoDB:          8.0.3
Using Mongosh:          2.3.3

For mongosh info see: https://www.mongodb.com/docs/mongodb-shell/

------
   The server generated these startup warnings when booting
   2024-11-06T15:02:45.447+05:30: Access control is not enabled for the database. Read and write access to data and configuration is unrestricted
------

test> show dbs
Employes  72.00 KiB
Mongodb   72.00 KiB
admin     40.00 KiB
config    60.00 KiB
local     40.00 KiB
test      40.00 KiB
test> use Mongodb
switched to db Mongodb
Mongodb> show collections
students
Mongodb> db.students.find()
[
  { _id: ObjectId('672b595e64292dc1f00d8190'), name: 'Sam', Div: 'B' },
  { _id: ObjectId('672cd186c87fbaf3810d8190'), name: 'abc' },
  { _id: ObjectId('672cd20fc87fbaf3810d8191'), name: 'abc' },
  { _id: ObjectId('672cd20fc87fbaf3810d8192'), age: 'C' }
]
Mongodb> db.students.insertOne({name:"abhi"})
{
  acknowledged: true,
  insertedId: ObjectId('672f1b646fb0511fe80d8190')
}
Mongodb> db.student.find()

Mongodb> db.students.find()
[
  { _id: ObjectId('672b595e64292dc1f00d8190'), name: 'Sam', Div: 'B' },
  { _id: ObjectId('672cd186c87fbaf3810d8190'), name: 'abc' },
  { _id: ObjectId('672cd20fc87fbaf3810d8191'), name: 'abc' },
  { _id: ObjectId('672cd20fc87fbaf3810d8192'), age: 'C' },
  { _id: ObjectId('672f1b646fb0511fe80d8190'), name: 'abhi' }
]
Mongodb> db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
...
...
... db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
Uncaught:
SyntaxError: Unexpected token, expected "," (4:0)

  2 |
  3 |
> 4 | db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
    | ^
  5 |

Mongodb> db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
... db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
Uncaught:
SyntaxError: Unexpected token, expected "," (2:0)

  1 | db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
> 2 | db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}
    | ^
  3 |

Mongodb> db.students.updateMany({name:"abhi"},{$set:{name:"Abhishek"}})

{
  acknowledged: true,
  insertedId: null,
  matchedCount: 1,
  modifiedCount: 1,
  upsertedCount: 0
}
Mongodb> db.students.find()
[
  { _id: ObjectId('672b595e64292dc1f00d8190'), name: 'Sam', Div: 'B' },
  { _id: ObjectId('672cd186c87fbaf3810d8190'), name: 'abc' },
  { _id: ObjectId('672cd20fc87fbaf3810d8191'), name: 'abc' },
  { _id: ObjectId('672cd20fc87fbaf3810d8192'), age: 'C' },
  { _id: ObjectId('672f1b646fb0511fe80d8190'), name: 'Abhishek' }
]
Mongodb>
    name: 'DEEPIKA',
    Role: 'SDE'
  },
  { _id: ObjectId('672b5bb9e053edfeb80d8191'), name: 'ABS', Div: 'B' }
]
Employes>
