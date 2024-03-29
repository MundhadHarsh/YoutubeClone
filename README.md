# VueTube RESTful API - YouTube Clone

> VueTube is a YouTube clone built with nodejs, expressjs & mongodb.

## Features

> CRUD (Create, Read, Update And Delete)

- Authentication with JWT (Reset Password with email)
  - Login (User/Admin)
  - Register
  - Forgot Password
- Pagination and search where necessary
- API Security (NoSQL Injections, XSS Attacks, http param pollution etc)
- Video (CRUD)
  - Upload video
  - Upload video thumbnail
  - Watch video
  - Increase Views
  - Like and dislike video
  - Comment & reply for video
  - Update video details
  - Delete video
- Subscribe to a channel
- View liked videos
- Subscriptions
- History (CRUD)
  - Watch history
  - Search history
- Settings
  - Modify channel name and email
  - Change password
  - Upload channel avatar


## Requirement

- NodeJS
- MongoDB

## Configuration File

Rename the config/.env.example to .env, then modify to your environment variables, mongodb uri, set your JWT_SECRET and SMTP variables

```ENV
NODE_ENV=development
PORT=3001

MONGO_URI=YOUR_URL

JWT_SECRET=YOUR_SECRET
JWT_EXPIRE=30d
JWT_COOKIE_EXPIRE=30

FILE_UPLOAD_PATH = ./public/uploads
MAX_FILE_UPLOAD = 1000000

SMTP_HOST=smtp.mailtrap.io
SMTP_PORT=2525
SMTP_EMAIL=
SMTP_PASSWORD=


```


## Installation

Install all npm dependecies

```console
npm install
```

Install nodemon globally

```console
npm install -g nodemon
```

### Note

Make sure you run the seeder to get categories in your database or Create a user with the role admin, then add category with the category endpoint.

Run database seeder

- Seeder folder is \_data/
- Edit the seeder file if you want to

```console
node seeder -i
```

Delete all data

```console
node seeder -d
```

## Start web server

```console
node run dev
```


## Developed by Harsh Mundhada

gmail [@mailId](harshmundhada@gmail.com)
Linkedin[@linkedin](https://www.linkedin.com/in/harsh-mundhada-473864229)