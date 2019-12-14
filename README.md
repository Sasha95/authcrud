dotnet run

```javascript
POST
http://localhost:4000/users/register
{
    "firstName": "Jason",
    "lastName": "Watmore",
    "username": "jason",
    "password": "my-super-secret-password"
}

POST
http://localhost:4000/users/authenticate

{
    "username": "jason",
    "password": "my-super-secret-password"
}

GET
http://localhost:4000/users
Headers (bulk Edit)
Authorization:Bearer <auth_token>


PUT
http://localhost:4000/users/1

{
    "firstName": "Foo",
    "lastName": "Bar"
}

Headers (bulk edit)
Content-Type:application/json
Authorization:Bearer <auth_token>