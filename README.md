# MONGODB-INTRODUCTION

first_name

last_name

email

gender

ip_address

age

show dbs
use mongodb_introduction
show collections

   <!-- insert one documnet  -->

db.users.insert({"first_name":"magendran","last_name":"anandhan","email":"magendran@gmail.com","gender":"male","ip_address":"2345",age:2})

     <!-- insert many document  -->

db.users.insertMany([{"first_name":"magendran","last_name":"anandhan","email":"magendran@gmail.com","gender":"male","ip_address":"2345",age:2},{"first_name":"kishore","last_name":"anandhan","email":"kishore@gmail.com","gender":"male","ip_address":"2345",age:22}])

db.users.insertMany([{"first_name":"venkat","last_name":"anandhan","email":"venkat@gmail.com","gender":"male","ip_address":"2345",age:2},{"first_name":"murali","last_name":"anandhan","email":"murali@gmail.com","gender":"male","ip_address":"2345",age:22},{"first_name":"pavani","last_name":"anandhan","email":"pavani@gmail.com","gender":"Female","ip_address":"2345",age:2}])
db.users.find()
db.users.findOne()

db.users.update({ "\_id" : ObjectId("62262f63db6ad5eec5a72508"}, {$set:{"first_name" : "anusha"}})

db.users.updateMany({ "first_name" : "arjun"}, {$set:{"first_name" : "malik"}})

db.users.updateMany([{{ "_id" : ObjectId("62262f63db6ad5eec5a72508")},{"first_name":"raja"}},{{ "_id" : ObjectId("62262f63db6ad5eec5a72507")},{"first_name":"thyagararaja"}},{{ "_id" : ObjectId("62262f06db6ad5eec5a72506")},{"first_name":"nirmala"}])

db.users.updateMany({"first_name" : "maggi"},{"$set" : {"eligible":"true"}})

dd.users.

users
db.users.delete()
