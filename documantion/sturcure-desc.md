## Architecture

![Architecture](/documantion/shots/udagram-api-hosting.png)

The front and backend is running on AMS (Amazon Web Services).

### Web hosting

![s3](/documantion/shots/amazon%20s3%20bucket.png)

The application Udagram:

- Frontend build with Angular
- User registration and login is supported with Bcryptjs and JWT token

the app is hosted on S3 Bucket & case a user creates a post the files are uploaded in the same place (but currentlly is not available).

### Database

![database](/documantion/shots/Amzon%20RDS%20database.png.png)

The database RDS created to init PostgreSQl db, To store user credentials and login infos are stored.
The db listening on PORT 5432.

### Server/Environment

![eb](/documantion/shots/Amazon%20Elastic%20Beanstalk%20env.png)

The server is built with Node.js and Express.

The app is deployed with Elastic Beanstalk , which allows this app to run on AWS cloud services. Through this deployment process an environment is created where the connection between EC2 (Elastic Compute Cloud) for server hosting and S3 is made.
