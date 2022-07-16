# Udagram Application [![CircleCI](https://circleci.com/gh/mahmoud-bebars/Udagram-deployment-process.svg?style=shield)](https://circleci.com/gh/circleci/Udagram-deployment-process)

## Description

the Application made for peoplpe to share some feed on it after creating account & login in to it

## Puplic web app url

you can visit the application from here ---> [Udagram](http://udagramfrontendbucket.s3-website-us-east-1.amazonaws.com) https://img.shields.io/endpoint?url=<URL>&style<STYLE>

## Application diagram

![diagram](./docs/udagram-api-hosting.png 'The Hosting Diagram')

## Docs Folder contains the following

- Aws RDS datbase sucess screenShot
- Aws Elastic beanstalk Env info & OK Health status confirmation
- Aws S3 Bucket ScreenShot info
- the udagra API hosting diagram
- cicleci pipleine pass passing the testing & the deploying with authorization confiromation for the repo
- Env variables passed to the circleci dashboard

## Techs & dependencies used in the application

### First: Front-End UI

- `ionic app`.
- Built with `Angular` framework.
- Coded in `Typescript` mode & built by comping to `js`.
- `SCSS` is used for styling.
- the UI is hosted with `AWS services` which is
  - An `S3 Bucket` to hold the Web App UI

### Second: Back-End API

- `Docker` is used to hold the application
- The API is Written with `TypeScript` for more security of types & code quality assurance.
- API is built With `Node.Js` & `Express.Js`
- Database used in the project is `Postgres` by :-
  - the pg package to set up db.
  - `sequelize` pacakage to set up sqls strings.
  - `db-migrate` for best collacaboration practices.
- `jsonwebtoken` to set up Authorization & autantication.
- for passwords encryption We used `bycrypt.js`.
- `email-validator` is used for email verfiying.
- The API is hosted with `AWS services` which is :-
  - `RDS` to Create the Database.
  - `Elastic BeanStalk` to SetUp the Environment of the Application & hold the Server.

## Deplyoment Process

- For Best Continous Integration We used `CircleCi` To init & deploy Our App

## Pipeline process

- starting with setup the environment
- preparing Env variables
- install nodejs in the circleci server
- install AWS CLI
- configure the AWS access key ID
- setup elastic beanstalk CLI
- Checkout the code
- install the backend API Dependencies
- build the Backend API
- install the front-end App Dependencies
- Build the front-end App
- Deploy the front-end App
- deploy the back-end API
