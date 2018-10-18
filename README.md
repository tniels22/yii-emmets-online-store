# yii-emmets-online-store
Yii Online Store Project - BYU Interview

# Resources:
1. Products
2. Users
3. Session

# Rest End Points

request | Path | Method
----|----|----
LIST| /Products| GET
RETRIEVE | /Products/id| GET
CREATE| /Products| POST
UPDATE | /Products/id|PUT
DEL| /Products/id| DELETE
RETRIEVE | /Session | GET
CREATE | /Session | POST
DELETE | /Session | DELETE
CREATE | /users | POST


# User Attributes:
1. _id
2. fName
3. lName
4. email
5. password

# Product Attributes:
1. _id
2. name
3. picture
4. description

# Session Attributes:
1. _id

# Schema
```
var productSchema = new mongoose.Schema({
  name: String,
  picture: String,
  description: String
});

var userSchema = new mongoose.Schema({
  fname: String,
  lname: String,
  email: String,
  encryptedPassword: String
});
```
