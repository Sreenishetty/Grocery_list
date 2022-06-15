# Grocery_list

Code is to maintain the grocery list of items
<!--  -->
Database used here is Mongodb
<!--  -->
For testing Postman is used
<!--  -->
For Routing FastApi is used
Routes:
  GET
  POST
  PUT 
  DELETE
  DELETE - ALSO USED FOR DELETING THE ENTIRE CART
  
  
 Mongodb Connection
 
 ### always do the connection in try except
###########################################
# Connecting  with MongoDB database
try:
    mongo = pymongo.MongoClient(
        host="localhost",
        port=27017,
        serverSelectionTimeoutMS = 1000
    )
    mongo.server_info() ## trigger  exception if cannot connect to database
    db = mongo.shopping
except:
    print("ERROR - Cannot connect  to  database")
 
