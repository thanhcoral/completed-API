# completed-API
completed API

## PIZZA DELIVERY API
This is a REST API for a Pizza delivery service

## ROUTES TO IMPLEMENT
| METHOD | ROUTE | FUNCTIONALITY |ACCESS|
| ------- | ----- | ------------- | ------------- |
| *POST* | ```/auth/signup/``` | _Register new user_| _All users_|
| *POST* | ```/auth/jwt/create/``` | _Login user_|_All users_|
| *POST* | ```/auth/jwt/refresh/``` | _Refresh the access token_|_All users_|
| *POST* | ```/auth/jwt/verify/``` | _Verify the validity of a token_|_All users_|
| *POST* | ```/orders/``` | _Place an order_|_All users_|
| *POST* | ```/orders/``` | _Get all orders_|_All users_|
| *GET* | ```/order/{order_id}/``` | _Retrieve an order_|_Superuser_|
| *PUT* | ```/orders/{order_id}/``` | _Update an order_|_All users_|
| *PUT* | ```/update-status/{order_id}/``` | _Update order status_|_Superuser_|
| *DELETE* | ```/delete/{order_id}/``` | _Delete/Remove an order_ |_All users_|
| *GET* | ```/user/{user_id}/orders/``` | _Get user's orders_|_All users_|
| *GET* | ```/user/{user_id}/order/{order_id}/``` | _Get user's specific order_|
| *GET* | ```/docs/``` | _View API documentation_|_All users_|

### tutorial
Turtorial
### init
- docker-compose run api django-admin startproject api .
- setup database
- docker-compose run api python manage.py makemigrations
- docker-compose run api python manage.py migrate
- docker-compose run api python manage.py createsuperuser

### up
- docker-compose up
- docker-compose down