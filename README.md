doctor-app consist of Rest API using Django Rest Framework.

Following are the features available in this app:

The doctor should be able to create an account using these informations : email, phone password, bithdate, gender,location,spoken languages,Diplomas,picture.
The doctor should be able to select many spoken languages.
The doctor should be able to log using a password (Two factor authentication is a plus).
The doctor should be able to modify his infomations.
The doctor should be able to add a patient with his first and last name ,birthdate, email.
The doctor should be able to list all his patients.

To run the project -

Windows:

Install virtual environment: 

	'pip install virtualenv'
	
	
Create a virtual environment: 

	'virtualenv venv(name_of_venv)'
	

Activate virtual environment

	source venv\Scripts\activate

Navigate to the directory

	cd doctor

Install the required packages

	pip install -r requirements.txt

Change the database settings in doctor/settings.py

Setting up your privacy using environment variables Create .env file and set below variables based on your configuration

	 PG_USERNAME=user_name_value
	 PG_PASSWORD=user_password
	 PG_HOST=server_host
	 PG_PORT=server_port
	 PG_DATABASE_NAME=database_name
	 
Run migrations

	python manage.py makemigrations
	python manage.py migrate

Start server

	python manage.py runserver 0.0.0.0:8000
	
Test the server with postman collection.

	Postman collection: https://www.getpostman.com/collections/9565f3d839376552e4c3
