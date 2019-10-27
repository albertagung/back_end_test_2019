# Classroom Registration API

This API is a dynamic Classroom and User registration process, which will be usefull for institution that needs a digital solution to help them solve registration process problem

## Auth User (optional):

### Login:
* URL: ```https://testing-255716.appspot.com/users/login```
* Method: ```POST```
* Body: 
	```
	{
		"username": "<USERNAME>",
		"password": "<PASSWORD>"
	}
	```

### Logout:
* URL: ```https://testing-255716.appspot.com/users/logout```
* Method: ```POST```
* Body: ```{}```

## CRUD Users:

### Create new user:
* URL: ```https://testing-255716.appspot.com/users/create```
* Method: ```POST```
* Body:
	```
	{
		"username": "<USERNAME>",
		"password": "<PASSWORD>",
		"name": "<USER_NAME>",
		"ClassroomId": <CLASSROOM_ID>
	}
	```

### Get all users: 
* URL: ```https://testing-255716.appspot.com/users```
* Method: ```GET```
* Body:```{}```

### Get user by id:
* URL: ```https://testing-255716.appspot.com/users/find/<ID_USER>```
* Method: ```GET```
* Body: ```{}```

### Update user:
* URL: ```https://testing-255716.appspot.com/users/update/<ID_USER>```
* Method: ```PUT```
*	Body: 
	```
	{
		"username": "<USERNAME>",
		<!-- If password null, then user is not updating their password -->
		<!-- If password not null, then user is going to update their password -->
		"password": "<PASSWORD> || NULL",
		"name": "<USER_NAME>",
		"ClassroomId": <CLASSROOM_ID>
	}
	```

### Remove user: 
* URL: ```https://testing-255716.appspot.com/users/remove/<ID_USER>```
* Method: ```DELETE```
*	Body: ```{}```


## CRUD Classrooms:

### Create new classroom: 
* URL: ```https://testing-255716.appspot.com/classrooms/create```
*	Method: ```POST```
*	Body: 
	```
	{
		"name": "<CLASSROOM_NAME>"
	}
	```

### Get all classrooms:
* URL: ```https://testing-255716.appspot.com/classrooms```
*	Method: ```GET```
*	Body: ```{}```

### Get classroom by id:
* URL: ```https://testing-255716.appspot.com/classrooms/find/<CLASS_ID>```
*	Method: ```GET```
*	Body: ```{}```

### Update classroom:
* URL: ```https://testing-255716.appspot.com/classrooms/update/<CLASS_ID>```
*	Method: ```PUT```
*	Body: 
	```	
	{
		"name": "<CLASSROOM_NAME>"
	}
	```

### Remove classroom:
* URL: ```https://testing-255716.appspot.com/classrooms/remove/<CLASS_ID>```
*	Method: ```DELETE```
*	Body: ```{}```
