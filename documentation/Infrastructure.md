# Udagram App Infrastructure

## Built With
this application was built with:-

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## Installation Pre-requistments
Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
2. IAM user with AmazonS3FullAccess and AdministratorAccess-AWSElasticBeanstalk permissions on AWS
3. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.

## Frondend Installation
1. cd udagram/udagram-frontend
2. npm install (to install all packages)
3. npm run test && npm run e2e (to run unit tests and end to end tests)
4. npm run lint (to linting the code)
5. npm run start to up the app on localhost 4200
6. npm run build (to generat build folder www)
7. npm run build --prod (to generat build folder www with production env variables that we use in deploying)
8. npm run deploy (to upload www folder to the s3 bucket)

## Backend Installation
1. cd udagram/udagram-api
2. npm install (to install all packages)
3. npm run dev to up the app on localhost 3000
4. npm run tsc (to transpile typescript to javascript)
5. npm run build (to generat build folder www)
6. npm run deploy (to upload www folder to the Elasticbeanstalk App)
