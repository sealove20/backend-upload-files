# backend-upload-files server

This is the back-end of the [frontend-upload-files
 project](https://github.com/sealove20/frontend-upload-files)

It's a image upload management app that supports only images smaller than 2mb. i've used two strategies to store the data using multer library to manage which one will be used. Local strategy was built using multer and is used in dev environment, while aws strategy was done with aws-sdk for nodeJS and is used in production environment.

# Getting Started

### Prerequisites

To run this project in the development mode, you'll need to have a basic environment with NodeJS 8+ installed. To use the database, you'll need to have MongoDB installed and running on your machine at the default port (27017) and also have a aws account to create a bucket used to store the photos.



You will need to create a **.env** file and create some environment variables like: 
  - APP_URL (Where the app will run, like localhost:3000...)
  - MONGO_URL
  - STORAGE (local or aws)
  - AWS_ACCESS_KEY_ID
  - AWS_SECRET_ACCESS_KEY
  - AWS_DEFAULT_REGION

### Installing

**Cloning the Repository**
```
$ git clone https://github.com/sealove20/backend-upload-files.git
$ cd backend-upload-files
```

**Installing dependencies**
```
$ yarn
```

__or__

```
$ npm install
```

**Running the server**
```
$ yarn start
```

__or__

```
$ npm run start
```


## Built With

- [NodeJS](https://nodejs.org/en/) 
- [express](https://expressjs.com/) 
- [MongoDB](https://www.mongodb.com/) 
- [mongoose](https://mongoosejs.com/) 
- [nodemon](https://nodemon.io/) 
- [dotenv](https://github.com/motdotla/dotenv) 
- [multer](https://github.com/expressjs/multer) 
