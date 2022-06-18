# M4-W4-P1
 Description
 E-COMMERCE FRONT PAGE & BACK OFFICE
 

Your goal is to create an e-commerce website with product management functionalities.

 

You'll have to implement:

- A front page, where the available products can be browsed

- A backoffice page, where a new product can be added to the list

 

In the backoffice page you'll have to implement a form for adding a new product to the website.

The shape of a product looks like this:

{
    "_id": "5d318e1a8541744830bef139",       // SERVER GENERATED
    "name": "3310 cellphone",                // REQUIRED
    "description": "An unforgettable icon.", // REQUIRED
    "brand": "Nokia",                        // REQUIRED
    "imageUrl": "https://bit.ly/3CExjRa",    // REQUIRED
    "price": 100,                            // REQUIRED
    "userId": "admin",                       // SERVER GENERATED
    "createdAt": "2021-09-19T09:32:10.535Z", // SERVER GENERATED
    "updatedAt": "2021-09-19T09:32:10.535Z", // SERVER GENERATED
    "__v": 0                                 // SERVER GENERATED
}
The REQUIRED fields are the only one you need to send with your request for creating a new one.

 

Your CRUD endpoint is:

https://striveschool-api.herokuapp.com/api/product/

This means you can GET and POST data from there.

 

🛑 IMPORTANT 🛑

EVERY REST API CALL SHOULD BE AUTHENTICATED.

Every request to the API should use Token Based Authentication to grant access permissions.

You can get your token by registering on: https://strive.school/studentlogin

 

Example:

fetch('https://striveschool-api.herokuapp.com/api/product/', {
	headers: {
		Authorization: 'Bearer XXXXXXXXXXXXXXXXX'
	}
})
Where `XXXXXXXXXXXXXXXXX` is the access token returned from the registration.

 

Tokens duration is set to 14 days.

Whenever you'll need to obtain a new one, you can send the following request:

method: "POST"
endpoint: "https://striveschool-api.herokuapp.com/api/account/login"
request body:
{
    "username": // the username you registered with,
    "password": // the password you registered with
}
 

Feel free to start from the attached Bootstrap template.

 
