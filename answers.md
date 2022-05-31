# Solutions sheet

Submit your final query after each iteration:

## Iteration 1
db.users.find({}, {name:1, _id:0})

## Iteration 2
db.users.find ({hasInsurance: {$eq: true }}, {namme:1})

## Iteration 3
db.users.find ({age: {$gte: 18 }}, {name:1})

## Iteration 4
db.users.findOne ({country: {$eq: "Italy" }}, {name:1, _id:0, email:1})

## Iteration 5
db.users.find({country: {$eq: "USA" }}, {name:1, _id:0}).limit(5)

## Iteration 6
db.users.find({phone:{$exists:true}},{name:1, _id:0})

## Iteration 7
db.users.updateOne({name: {$eq: "Marissa Geller"}}, {$set: {email: "marissa@hotmail.com"}})

## Iteration 8
db.users.updateMany({country:  {$eq: "UK"}}, {$set: {currency: "pounds"}})

## Iteration 9
db.users.find({country: {$eq: "UK"}}, {name:1, _id:0, currency:1})


## Iteration 10
db.users.deleteMany ({age: {$gte: 45 }})








