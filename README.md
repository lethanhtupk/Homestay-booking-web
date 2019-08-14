# Homestay Booking Web

This web application provide feature three kind of user
1. Normal user
2.Member 
3.Admin
The number of feature they can use base on their role in system. 

To run this application. You have to install mysql in your computer.and have a schema have the same name with DATABASE_NAME in homestay/.env file

Change the environment variable in homestay/.env file to match with your

To apply table in schema. Run command "python manage.py db init" and then "python manage.py db migrate"

To run server. Run command "python manage.py runserver" and open "127.0.0.1:5000" on your browser.

It also provide the API documentation. Help the developer can easy to test every endpoint in system.

![Screenshot (6)](https://user-images.githubusercontent.com/29749097/62989121-f3f44f80-be70-11e9-881f-75aba7dd080b.png)

In application. We have two kind of endpoint 
1. Security endpoint 
2. Normal endpoint

With security endpoint. To access this endpoint. You need to send an access token in header of request. This token you can recieve when you login the website

![1](https://user-images.githubusercontent.com/29749097/62989107-eb9c1480-be70-11e9-98e6-d1b6100b997f.jpg)

After you logout website. This access token will be revoke or after a period time. To recieve new access token. You can send a new login request or get new access token by refresh token you have been recieved when logged in.

The sytem also can identify the role of current user to give the user permission to do the feature they want or return a issue message

