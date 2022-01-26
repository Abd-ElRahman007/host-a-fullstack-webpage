# Udagram

## Getting Started

here we will go through the process of the project we will discuss the infrastructure, app dependencies and the pipeline process

## Infrastructure

these project uses angular, node, express, jasmine.
we set up a node environment to run the server and we connect the server with a (RDS) postgres database on (AWS) then the frontend uses the angular framework to build it, below are some useful links for them

the port that the database uses is (5430)

the Environment variables will be supplied via screenshots

### Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## App Dependencies

the app uses (bcrypt, bodyparser, cors, dontenv, email-validator, express, jsonwebtoken, pg[postgres], reflect-metadata, sequelize,angular, ionic, core-js, rxjs, zone,js) for production and uses (the types for [bluebird,cors,express,node,sequelize,validator,eslint,angular,ionic,jasmine,node]chai,mocha,ts-node,typescript,codelyzer,karma,protractor) the app uses typescript and jasmine and mocha for testing

## Pipeline process

the pipeline is configured with circleci to run with this repo when there is a new commit that is made the process is as follows

1. node get installed
2. aws-cli get setup
3. aws-elastic-beanstalk get setup
4. the frontend install dependencies
5. the backend install dependencies
6. the frontend builds
7. the backend builds
8. the backend deploys to elastic-beanstalk
9. the frontend deploys to s3

the badge for the pipeline build

[![CircleCI](https://circleci.com/gh/Abd-ElRahman007/host-a-fullstack-webpage.svg?style=svg)](https://circleci.com/gh/Abd-ElRahman007/host-a-fullstack-webpage)

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

## Link to the project

[click here](http://projectex12345if.s3-website-us-east-1.amazonaws.com)

### Unit Tests

Unit tests are using the Jasmine Framework.

### End to End Tests

The e2e tests are using Protractor and Jasmine.
