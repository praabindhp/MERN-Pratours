
# Pratours Project
![Pratours Logo](https://iili.io/HV96TF9.png)
## For The Adventure Lovers

The Pratours Is A Project Made In Node JavaScript Using Express, MongoDB Connection With Mongoose, Mailing Services Made By Nodemailer Using Sendgrid, Stripe For Payment, Mapbox For Map Integration And Many Other Functionalities.

## Project Snapshots

### Pratours Tour Overview
![Pratours Tour Overview](https://iili.io/HV96hAJ.png)

## What Is MERN - PRATOURS?
The Pratours is an impressive project built using Node.js and Express, a powerful JavaScript framework. It seamlessly integrates with MongoDB through the robust Mongoose library, providing efficient database connectivity and management. To enhance communication and engagement, the project incorporates mailing services powered by Nodemailer, utilizing SendGrid for reliable email delivery.

- Built using the MERN stack (MongoDB, Express.js, React.js, Node.js) for a full-stack web application.
- User authentication and authorization with features like signup, login, and password reset.
- Integration with MongoDB database using Mongoose for efficient data storage and retrieval.
- Seamless front-end development with React.js, providing a responsive and interactive user interface.
- User-friendly tour booking system with options to search, filter, and book tours based on preferences.
- Integration of Stripe payment gateway for secure and convenient online payments.
- Map integration using Mapbox to display interactive maps and provide location-based information.
- Email notifications and communication using Nodemailer and SendGrid for reliable mailing services.
- Advanced functionalities like user reviews and ratings for tours, allowing users to share their experiences.
- Comprehensive admin panel for managing tours, users, bookings, and other site content.
- Advanced search functionality to easily find desired tours based on location, date, price, etc.
- Implementation of features like pagination and sorting to enhance usability and performance.
- Error handling and validation mechanisms to ensure data integrity and a smooth user experience.
- Integration of various third-party APIs and libraries to enhance functionality and provide a seamless user experience.

These features collectively make the MERN Pratours project a comprehensive and feature-rich application for booking and managing tours, providing an enjoyable experience for both users and administrators.

### Pratours All Tours
![Pratours All Tours 1](https://iili.io/HV96z67.png)
![Pratours All Tours 2](https://iili.io/HV96CZl.png)

### Pratours Park Camper Tour Page
![Pratours Dedicated Tour Page](https://iili.io/HV96GF1.png)

### Pratours Sports Lover Tour Page
![Pratours Dedicated Tour Page](https://iili.io/HV96jwv.png)

### Pratours Login
![Pratours Login](https://iili.io/HV96uae.png)

### Pratours User Account
![Pratours User Account](https://iili.io/HV96hAJ.png)

### Pratours Admin Dashboard
![Pratours Admin Dashboard](https://iili.io/HV96Bj4.png)

### Pratours Admin Account
![Pratours Admin Account 1](https://iili.io/HV96KyG.png)
![Pratours Admin Account 2](https://iili.io/HV96quf.png)
![Pratours Admin Account 3](https://iili.io/HV96Fvs.png)

### Pratours Tour Description
![Pratours Tour Description](https://iili.io/HV96V8g.png)

### Pratours Dynamic Maps
![Pratours Dynamic Maps](https://iili.io/HV96Ryb.png)

### Pratours Dynamic Reviews
![Pratours Dynamic Reviews](https://iili.io/HV96A8u.png)

### Pratours Data Model
![Pratours Data Model](https://iili.io/HV96xGS.png)

### Pratours MongoDB Compass
![Pratours MongoDB Compass](https://iili.io/HV967uj.png)

### Pratours MongoDB Cloud
![Pratours MongoDB Cloud](https://iili.io/HV96aZQ.png)

### Pratours Code Structure
![Pratours Code Structure](https://iili.io/HV96on2.png)

### Pratours Backend Running Server
![Pratours Backend Running Server](https://iili.io/HV960MB.png)

### Pratours Postman Aliasing
![Pratours Postman Aliasing](https://iili.io/HV96lnV.png)

### Pratours Postman - Tour Sorting
![Pratours Postman Sort](https://iili.io/HV96wtR.png)

## API Reference

#### Tour API

API Reference For Tours And Its Operations

#### Get All Tours

```http
  GET /api/v1/tours
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |

#### Get Tour

```http
  GET /api/v1/tours/${id}
```

| Parameter | Type     | Description           |
| :-------- | :------- | :-------------------- |
| `id`      | `string` | **Required**. Tour ID |

#### Create A Tour

```http
  POST /api/v1/tours
```

| Parameter      | Type     | Description                           |
| :------------- | :------- | :------------------------------------ |
| `api_key`      | `string` | **Required**. Your API Key            |
| `name`         | `string` | **Required**. Tour Name               |
| `duration`     | `number` | **Required**. Tour Duration           |
| `maxGroupSize` | `number` | **Required**. Tour Maximum Group Size |
| `difficulty`   | `string` | **Required**. Tour Difficulty         |
| `price`        | `number` | **Required**. Tour Price              |
| `summary`      | `string` | **Required**. Tour Summary            |
| `imageCover`   | `string` | **Required**. Tour Image Cover        |

#### Update A Tour

```http
  PATCH /api/v1/tours/${id}
```

| Parameter    | Type     | Description                       |
| :----------- | :------- | :-------------------------------- |
| `api_key`    | `string` | **Required**. Your API Key        |
| `id`         | `string` | **Required**. Tour ID             |
| `imageCover` | `file`   | **Required**. Tour Image Cover    |
| `images`     | `file`   | **Required**. Tour Grid - 1 Image |
| `images`     | `file`   | **Required**. Tour Grid - 2 Image |
| `images`     | `file`   | **Required**. Tour Grid - 3 Image |
| `price`      | `number` | **Required**. Tour Price          |

#### Delete A Tour

```http
  DELETE /api/v1/tours/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `id`      | `string` | **Required**. Tour ID      |

#### Get Top 5 Cheap Tours

```http
  GET /api/v1/tours/top-5-cheap
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |

#### Get Monthly Plan

```http
  GET /api/v1/tours/top-5-cheap
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |

#### Get Tour Stats

```http
  GET /api/v1/tours/tour-stats
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |

#### Get Tours Within Radius

```http
  GET /api/v1/tours/tours-within/{distance}/center/${{longitude},{latitude}}/unit/${unit}
```

| Parameter   | Type     | Description                       |
| :---------- | :------- | :-------------------------------- |
| `api_key`   | `string` | **Required**. Your API Key        |
| `distance`  | `string` | **Required**. Your Distance       |
| `longitude` | `string` | **Required**. Your Longitude      |
| `latitude`  | `string` | **Required**. Your Latitude       |
| `unit`      | `string` | **Required**. Your Preferred Unit |

#### Get Distances to Tours From Point

```http
  GET /api/v1/tours/{distance}/center/${longitude}},${latitude}}/unit/${unit}
```

| Parameter   | Type     | Description                       |
| :---------- | :------- | :-------------------------------- |
| `api_key`   | `string` | **Required**. Your API Key        |
| `distance`  | `string` | **Required**. Your Distance       |
| `longitude` | `string` | **Required**. Your Longitude      |
| `latitude`  | `string` | **Required**. Your Latitude       |
| `unit`      | `string` | **Required**. Your Preferred Unit |

#### User API

API Reference For Users And Its Operations

#### Get All Users

```http
  GET /api/v1/users
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |

#### Get A User

```http
  GET /api/v1/users/${id}
```

| Parameter | Type     | Description           |
| :-------- | :------- | :-------------------- |
| `id`      | `string` | **Required**. User ID |

#### Update A User

```http
  PATCH /api/v1/users/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `id`      | `string` | **Required**. User ID      |
| `name`    | `string` | **Required**. User Name    |
| `email`   | `string` | **Required**. User Email   |

#### Delete A Tour

```http
  DELETE /api/v1/users/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `id`      | `string` | **Required**. User ID      |

#### Get Current User

```http
  GET /api/v1/users/me
```

| Parameter | Type    | Description           |
| :-------- | :------ | :-------------------- |
| `jwt`     | `token` | **Required**. User ID |

#### Update Current User

```http
  PATCH /api/v1/users/updateMe
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `id`      | `string` | **Required**. User ID      |
| `name`    | `string` | **Required**. User Name    |
| `email`   | `string` | **Required**. User Email   |
| `photo`   | `file`   | **Required**. User Picture |

#### Delete Current User

```http
  GET /api/v1/users/deleteMe
```

| Parameter | Type    | Description           |
| :-------- | :------ | :-------------------- |
| `jwt`     | `token` | **Required**. User ID |

#### Authentication API

API Reference For User Authentication And User Functionalities

#### Update Current User

```http
  POST /api/v1/users/signup
```

| Parameter         | Type       | Description                    |
| :---------------- | :--------- | :----------------------------- |
| `api_key`         | `string`   | **Required**. Your API Key     |
| `name`            | `string`   | **Required**. User Name        |
| `email`           | `string`   | **Required**. User Email       |
| `password`        | `password` | **Required**. User Password    |
| `passwordConfirm` | `password` | **Required**. Confirm Password |

#### Update Current User

```http
  POST /api/v1/users/login
```

| Parameter  | Type       | Description                 |
| :--------- | :--------- | :-------------------------- |
| `api_key`  | `string`   | **Required**. Your API Key  |
| `email`    | `string`   | **Required**. User Email    |
| `password` | `password` | **Required**. User Password |

#### Forgot Password

```http
  POST /api/v1/users/forgotPassword
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `email`   | `string` | **Required**. User Email   |

#### Reset Password

```http
  POST /api/v1/users/resetPassword
```

| Parameter         | Type       | Description                    |
| :---------------- | :--------- | :----------------------------- |
| `password`        | `password` | **Required**. User Password    |
| `passwordConfirm` | `password` | **Required**. Confirm Password |

#### Update Current User Password

```http
  PATCH /api/v1/users/updateMyPassword
```

| Parameter         | Type       | Description                        |
| :---------------- | :--------- | :--------------------------------- |
| `passwordCurrent` | `password` | **Required**. Current Password     |
| `password`        | `password` | **Required**. User New Password    |
| `passwordConfirm` | `password` | **Required**. Confirm New Password |

#### Reviews API

API Reference For Reviews And Its Operations

#### Get All Reviews

```http
  GET /api/v1/reviews
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |

#### Get A Review

```http
  GET /api/v1/reviews/${id}
```

| Parameter | Type     | Description             |
| :-------- | :------- | :---------------------- |
| `id`      | `string` | **Required**. Review ID |

#### Create A Review

```http
  POST /api/v1/reviews
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `review`  | `string` | **Required**. Tour Review  |
| `rating`  | `number` | **Required**. Tour Rating  |
| `tour`    | `id`     | **Required**. Tour ID      |
| `user`    | `id`     | **Required**. User ID      |

#### Update A Review

```http
  PATCH /api/v1/reviews/${id}
```

| Parameter | Type     | Description                  |
| :-------- | :------- | :--------------------------- |
| `api_key` | `string` | **Required**. Your API Key   |
| `id`      | `string` | **Required**. Review ID      |
| `rating`  | `number` | **Required**. Rating Changes |

#### Delete A Review

```http
  DELETE /api/v1/reviews/${id}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `api_key` | `string` | **Required**. Your API Key |
| `id`      | `string` | **Required**. Review ID    |

#### Tours / Reviews API
API Reference For Reviews And Its Operations

#### Get All Reviews On A Tour

```http
  GET /api/v1/tours/${id}/reviews
```

| Parameter | Type     | Description                  |
| :-------- | :------- | :--------------------------- |
| `api_key` | `string` | **Required**. Your API Key   |
| `id`      | `string` | **Required**. Tour ID        |

#### Create New Review On Tour

```http
  POST /api/v1/tours/${id}/reviews
```

| Parameter | Type     | Description                  |
| :-------- | :------- | :--------------------------- |
| `api_key` | `string` | **Required**. Your API Key   |
| `id`      | `string` | **Required**. Tour ID        |
| `rating`  | `number` | **Required**. Rating Changes |
| `review`  | `string` | **Required**. Review Changes |

#### 3rd Party APIs
- MongoDB : For Database
- Mapbox API : For Mapping Integration
- Stripe API : For Payment Integration
- Sendgrid : For Production Email Integration
- Mailtrap : For Testing Email Integration

## Deployment

Installation Of The Project

```bash
  sudo apt install nodejs
  sudo apt install npm
  npm init
  npm install
  npm start
```

Scripts For The Project

```bash
  start - "nodemon server.js"
  start:prod - "NODE_ENV=production nodemon server.js"
  debug - "ndb server.js"
  watch:js - "parcel watch ./public/js/index.js --out-dir ./public/js --out-file bundle.js"
  build:js - "parcel watch ./public/js/index.js --out-dir ./public/js --out-file bundle.js"
```

## Dependencies

Dependencies For The Project

```bash
  @babel/polyfill : "^7.4.4"
  axios : "^1.3.4"
  bcrypt0js : "^2.4.3"
  cookie-parser : "^1.4.4"
  dotenv : "^7.0.0"
  express : "^4.16.4"
  express-mongo-sanitize : "^1.3.2"
  express-rate-limit : "^3.5.0"
  helmet : "^3.16.0"
  hpp : "^0.2.2"
  jsonwebtoken : "^9.0.0"
  mongoose : "^5.5.2"
  morgan : "^1.9.1"
  nodemailer : "^6.1.1"
  pug : "^3.0.2"
  slugify : "^1.3.4"
  validator : "^13.9.0"
  xss-clean : "^0.1.1"
```

Dev Dependencies For The Project

```bash
  eslint : "^5.16.0",
  eslint-config-airbnb : "^17.1.0",
  eslint-config-prettier : "^4.1.0",
  eslint-plugin-import : "^2.17.2",
  eslint-plugin-jsx-a11y : "^6.2.1",
  eslint-plugin-node : "^8.0.1",
  eslint-plugin-prettier : "^3.0.1",
  eslint-plugin-react : "^7.12.4",
  parcel-bundler : "^1.8.1",
  prettier : "^1.17.0"
```

Engine Dependency For The Project

```bash
  node: ">=10.0.0"
```

## Authors

- Praabindh Pradeep - [@praabindhp](https://www.github.com/praabindhp)
- Praabindh P - [@praabindh](https://www.github.com/praabindh)

Built During The Internship Phase Of Product Engineer In [Codingmart Technologies](https://codingmart.com/), Coimbatore, Tamil Nadu, India.