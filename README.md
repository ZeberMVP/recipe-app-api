# Recipe API
This is a Django Rest Framework-powered API that allows users to add recipes with their ingredients. The project was developed using a test-driven development approach, with exhaustive unit tests for all functionalities. The API documentation was generated with drf-spectacular.

## Deployment
You can access the deployed project on AWS by following this link: [/api/docs/](http://ec2-13-38-93-0.eu-west-3.compute.amazonaws.com/api/docs/)

## Local Installation
If you want to deploy this locally through Docker, follow this steps:

1. Install Docker if you haven't already and start it.

2. Clone this repository.

3. In your terminal, navigate to the repository's root directory.

4. Rename the <b>`.env.sample`</b> file to <b>`.env`</b> and modify the password.

5. Run the following commands: <br> <br>
`docker-compose build` <br> <br>
`docker-compose up`

6. Create a superuser: <br> <br>
`docker-compose run --rm app sh -c "python manage.py createsuperuser"` <br> <br>

7. Go to <b>`http://127.0.0.1:8000/admin/`</b> and log in with your superuser account.

![image](https://user-images.githubusercontent.com/106594858/235707598-fa1d0e40-7854-4b9f-84d9-53bbaebdffa8.png)

![image](https://user-images.githubusercontent.com/106594858/235708685-57cff312-17d8-4b69-af88-5743274e4dab.png)



Congratulations! You have successfully deployed the project locally.

## API Routes

The API documentation is available through Swagger API. To access it, go to <b>`/api/docs/`</b> and browse the available routes and their descriptions. <br> <br>

Note that users must be authenticated with a token before adding new recipes.

![image](https://user-images.githubusercontent.com/106594858/235707408-c9dc990b-3cf8-4582-b1fa-baf907c432f8.png)
