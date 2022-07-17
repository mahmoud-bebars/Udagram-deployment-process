## Dependencies

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
