# Students | Requests | Response | Route (web|api) | Controller | Factories | Migrations | Migrate | Seeders 
<!-- [Live Link](https://bmi-calculator-ostad.netlify.app) -->

The Students is a simple Laravel project and updated versioin. I include Requests | Response | Route (web|api) | Controller | Factories | Migrations | Migrate | Seeders.

And it's assignment projects of PHP and Larvel of OSTAD.

![wellcome project](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/wellcome.png)

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Document of assignment projects of this project](#document-of-assignment-projects-of-this-project)
- [Laravel Folder Structure](#laravel-folder-structure)
- [Simple Route](#simple-route)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Description

The Students is a simple Laravel project and updated versioin. I include Requests | Response | Route (web|api) | Controller | Factories | Migrations | Migrate | Seeders.

## Features
| Key Features                | Description                                                  |
| ---------------------------| ------------------------------------------------------------ | 
|  Laravel Installation  | Laravel Properly Installed |
|  Folder Structure     | Explain Properly of Folder Structure |
|  Routing     | Baic Routing Explain |


## Demo
Project Home Page

[![Demo Video](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/wellcome.png)](https://youtu.be/RYAh3rSyWHs)

## Technologies Used

List the technologies, libraries, frameworks, or languages that you used to build your project. You can also provide links to their official websites or documentation.

- Laravel
## Installation

Clone the repository to your local machine

bash

    git clone https://github.com/ahmmedsabbirbd/students.git

Open Project folder:

bash

     cd students

Install the necessary dependencies by running the following command in the project directory:

bash

     composer install

This will install all the required packages and dependencies needed to run the project.
Create a .env file in the root of the project and add the required environment variables. These variables may include database credentials, API keys, and other configuration details. You can find the list of required environment variables in the project's README.md file.
Start the development server by running the following command:

bash

    php artisan serve

This will start the server and the application will be available at http://localhost:8000/.

Note: If you encounter any issues while installing or running the project locally, please refer to the project's documentation or reach out to the project maintainers for assistance.

## Document of assignment projects of this project

1. ## Question 1:
     `You have a Laravel application with a form that submits user information using a `POST` request. Write the code to retrieve the 'name' input field value from the request and store it in a variable called $name.`

     I create a controller and i decleare object instance "Request $request" and i accept "$request->input('name') as $name value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-1.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-1.png)

2. ## Question 2:
     `In your Laravel application, you want to retrieve the value of the `'User-Agent'` header from the current request. Write the code to accomplish this and store the value in a variable called `$userAgent.``

     I create a controller and i decleare object instance "Request $request" and i accept "$request->header('User-Agent') as $userAgent value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-w-2.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-2.png)
3. ## Question 3:
     `You are building an API endpoint in Laravel that accepts a GET request with a `'page'` query parameter. Write the code to retrieve the value of the 'page' parameter from the current request and store it in a variable called `$page`. If the parameter is not present, set `$page` to `null`.`
     
     I create a controller and i decleare object instance "Request $request" and i accept "$request->query('page') as $page value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-w-3.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-3.png)
4. ## Question 4:
     
     Create a JSON response in Laravel with the following data:

          {
               "message": "Success",
               "data": {
                    "name": "John Doe",
                    "age": 25
               }    
          }
     
     I create a controller, it's StudentController and I have singleIndext method and i return single student data.

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-w-4.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-4.png)
5. ## Question 5:
     
     `You are implementing a file upload feature in your Laravel application. Write the code to handle a file upload named `'avatar'` in the current `request` and store the uploaded file in the `'public/uploads'` directory. Use the `original filename` for the uploaded file.`
     
     I create a controller and i decleare object instance "Request $request" and i accept "$request->file('avatar') as $avatar value and i get photo current name name (getClientOriginalName()) this method in php laravel and uploaded photo my "public/upload" "$avatar->move(public_path('/uploads'), $avatarName);" this method

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-w-5.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-5.png)

6. ## Question 6:
     
     `Retrieve the value of the `'remember_token'` cookie from the current request in Laravel and store it in a variable called `$rememberToken.` If the cookie is not present, set $rememberToken to null.`
     
     I create a controller and i decleare object instance "Request $request" and i accept "$request->cookie('remember_token') as $rememberToken value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-w-6.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-6-v1.png)
     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-6-v2.png)
7. ## Question 7:
     
     `Create a route in Laravel that handles a `POST` request to the `'/submit'` URL. Inside the route closure, retrieve the `'email'` input parameter from the request and store it in a variable called `$email`. Return a JSON response with the following data:`


          {


          "success": true,


          "message": "Form submitted successfully."


          }
     
     I create SubmitController and i decleare object instance "Request $request" and i accept "$request->input('email') and store it $email value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-w-7.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/assignment_q-p-7.png)
 

## Laravel Folder Structure
     
![Laravel Folder Structure](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/folder-structure.png)

1. ### `app`:
     This folder contains the core of your Laravel application, including its models, controllers, service providers, and other application-specific code.

2. ### `bootstrap`:
     This folder contains files that are responsible for bootstrapping your Laravel application, including the app.php file which loads the application's configuration files and service providers.
3. ### `config`:
     This folder contains configuration files for your application, including database configuration, app configuration, and other configuration files.
4. ### `database`:
     This folder contains database-related files, including migration files, seed files, and the database itself.
     This folder contains configuration files for your application, including database configuration, app configuration, and other configuration files.
5. ### `public`:
     This folder contains the public-facing files for your Laravel application, including the index.php file which serves as the entry point for all incoming requests.
6. ### `resources`:
     This folder contains the assets and templates for your application, including views, language files, and asset files such as CSS and JavaScript files.
7. ### `routes`:
     This folder contains the routes for your application, including the web.php file which defines the routes for your application's web interface and the api.php file which defines the routes for your application's API.
8. ### `storage`:
     This folder contains files that are generated by your Laravel application, including log files, cache files, and session files.
9. ### `tests`:
     This folder contains test files for your application, including unit tests and feature tests.
10. ### `vendor`:
     This folder contains all of the third-party packages that your Laravel application depends on, including the Laravel framework itself.


## Simple Route

1. ### I create simple route and it's named "world".

     ![Simple Route](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/world.png)

2. ### return "Hello, World".

     ![Simple Route Output](https://raw.githubusercontent.com/ahmmedsabbirbd/book/master/public/assets/documentation/world-output.png)
## Usage

### Getting Started
To get started with Book, you will need to follow the installation instructions in the previous section.

## API Documentation
Did not Provide any API

## Contributing

Contributions to our project are welcome and encouraged! To get started, please read our CONTRIBUTING.md file, which outlines our guidelines for contributing, reporting issues, and suggesting new features.

1. ### In general, contributors can help by:
    Reporting bugs or issues they encounter.
    Fixing bugs or implementing new features.
    Providing feedback and suggestions for improving the project.
    Writing tests and improving documentation.

2. ### To contribute to the project, please follow these steps:
    Fork the repository on GitHub.
    Create a new branch with a descriptive name for your contribution.
    Make your changes and test them thoroughly.
    Create a pull request to merge your changes back into the main branch of the project.
    Wait for your changes to be reviewed and merged.

    Please note that all contributions are subject to our code of conduct, and we ask that all contributors follow our guidelines for contributing. If you have any questions or concerns, please don't hesitate to reach out to the project maintainers.

    We appreciate your interest in contributing to our project and look forward to working with you!

## License
Any one use it

## Contact

If you have any questions, feedback, or suggestions, feel free to contact us using the following methods:

- Email: ahmmedsabbirbd@gmail.com
- Linkdin: [ahmmedsabbirbd](https://www.linkedin.com/in/ahmmedsabbirbd/)
- Website: [Portfolio](https://sabbir-me.netlify.app)

We appreciate your interest in our project and look forward to hearing from you!