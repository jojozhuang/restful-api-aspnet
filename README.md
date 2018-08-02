# Restful API
RESTful API for CRUD operations, developed with ASP.NET Core.

# Function
Six RESTful APIs for the Game Store web application.

API                       | Description         | URL
--------------------------|---------------------|--------------
GET /api/products         | Get all products    | GET [http://localhost:8080/api/products](http://localhost:8080/api/products)
GET /api/products/{id}    | Get a product by ID | GET [http://localhost:8080/api/products/1](http://localhost:8080/api/products/1)
POST /api/products        | Add a new product   | POST [http://localhost:8080/api/products](http://localhost:8080/api/products)
PUT /api/products/{id}    | Update a product    | PUT [http://localhost:8080/api/products/1](http://localhost:8080/api/products/1)
DELETE /api/products/{id} | Delete a product    | DELETE [http://localhost:8080/api/products/1](http://localhost:8080/api/products/1)
POST /api/upload          | Upload an image     | POST [http://localhost:8080/api/upload](http://localhost:8080/api/upload)

# Setup Locally
```bash
git clone https://github.com/jojozhuang/restful-api-aspnet.git
```
Open the solution file with Microsoft Visual Studio, compile and run. Access http://localhost:8080/api/products in web browser or PostMan, you should get the following json as response.
```json
[  
   {  
      "id":3,
      "productName":"Wireless Controller",
      "price":19.99,
      "image":"http://localhost:8080/images/controller.jpg"
   },
   {  
      "id":2,
      "productName":"Wii",
      "price":269.0,
      "image":"http://localhost:8080/images/wii.jpg"
   },
   {  
      "id":1,
      "productName":"Xbox 360",
      "price":299.0,
      "image":"http://localhost:8080/images/xbox360.jpg"
   }
]
```

# Deploy to Azure
Follow tutorial [Deploying RESTful API to Azure](http://jojozhuang.github.io/tutorial/restful/deploying-restful-api-to-azure/) to deploy it to [Azure](https://portal.azure.com/).

The available RESTful API on Azure is
* baseURL: https://gamestore-api.azurewebsites.net/

For example, call https://gamestore-api.azurewebsites.net/api/products to get all products.

# Portfolio
Read portfolio [Game Store(Angular)](https://jojozhuang.github.io/portfolio/game-store-angular/) or [Game Store(React)](http://jojozhuang.github.io/portfolio/game-store-react/) to learn how these RESTful APIs are consumed by Angular and React applications.

# Tutorial
Read tutorial [Building RESTful APIs with ASP.NET Core](https://jojozhuang.github.io/tutorial/react/building-restful-apis-with-aspnet-core/) to learn how this RESTful API is built.
