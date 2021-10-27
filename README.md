## Mock Login REST API

### Getting Started
Install dependencies
```
npm install
```

Run the app
```
node index.js
```

### Docker
Build the image
```
docker build . -t mock-login-api/mock-login-api
```

Run the image
```
docker run -p 9001:9001 -d mock-login-api/mock-login-api
```

### Endpoints

#### 1. Login user
> /user/login

POST

Payload:
```
{
    "username": "osh@handal.dev",
    "password": "osh@handal.dev"
}
```
Response:
```
{
    "userId": "1908789",
    "username": "osh@handal.dev",
    "name": "Osh Pilaf",
    "lastLogin": "3 March 2020 03:38 PM",
    "email": "osh@handal.dev"
}
```

#### 2. Get user by id
> /user/:id

GET

Payload:
- none

Response:
```
{
    "userId": "1908789",
    "username": "osh@handal.dev",
    "name": "Osh Pilaf",
    "lastLogin": "3 March 2020 03:38 PM",
    "email": "osh@handal.dev"
}
```