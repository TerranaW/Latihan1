# API DOCUMENTATION

# Authentication

## Register

- **Endpoint**: `POST /auth/register`
- **Description**: Register user baru.

  ### Request Body :
  ```json
  {
  "username": "example",
  "email": "example@example.com",
  "password": "password123",
  }
  
 ### Response Body :
  - **Status Code**: **201 (created)**
      ```json
      {
       "message" : "sucessfully registered"
      }
      
  - **Status Code**: **500 (Internal Server Error)**
     ```json
      {
       "message" : "Error registering user"
      }

     
## Log In

- **Endpoint**: `POST /auth/login`
- **Description**: Login User.

  ### Request Body :
  ```json
  {
  "username": "example",
  "password": "password123",
  }
  
 ### Response Body :
  - **Status Code**: **200 (ok)**
      ```json
      {
       "message" : "sucessfully logged in"
      }
      
  - **Status Code**: **404 (Not Found)**
     ```json
      {
       "message" : "User not found"
      }
     
  - **Status Code**: **401 (Unauthorized)**
    ```json
      {
       "message" : "Incorrect password"
      }
  - **Status Code**: **500 (Internal Sever Error**
    ```json
      {
       "message" : "Error Loging in"
      }

# Todo-List

## Get All Todo

- **Endpoint**: `GET /todos/`
- **Description**: Mengambil semua todo yang ada.
  
 ### Response Body :
  - **Status Code**: **200 (OK)**
      ```json
      {
       "message" : "sucessfully got all todos "
      }
      
  - **Status Code**: **500 (Internal Server Error)**
     ```json
      {
       "message" : "Error registering getting todos"
      }
     
 ## Get Todo By Id

- **Endpoint**: `GET /todos/:id`
- **Description**: Mengambil semua todo yang ada.
  
 ### Response Body :
  - **Status Code**: **200 (OK)**
      ```json
      {
       "message" : "sucessfully got todo by id "
      }
      
  - **Status Code**: **500 (Internal Server Error)**
     ```json
      {
       "message" : "Error registering getting todo id"
      }

 ## Add Todo 

- **Endpoint**: `POST /todos/`
- **Description**: Menambahkan Todo Baru.
  
 ### Response Body :
  - **Status Code**: **201 (created)**
      ```json
      {
       "message" : "Todo sucessfully added"
      }
      
  - **Status Code**: **500 (Internal Server Error)**
     ```json
      {
       "message" : "Error adding todo"
      }

## Add Todo Bulk

- **Endpoint**: `POST /todos/`
- **Description**: Menambahkan Todo Baru dalam jumlah banyak.
  
 ### Response Body :
  - **Status Code**: **201 (created)**
      ```json
      {
       "message" : "Todo sucessfully added"
      }
      
  - **Status Code**: **500 (Internal Server Error)**
     ```json
      {
       "message" : "Error adding todo"
      }
