# React App with Docker Support

This repository contains a React app that is dockerized for easy deployment. It includes a development Dockerfile and a production Dockerfile for building the app in different environments. There is also a docker-compose file for running the app locally in development mode, and another for deploying the app in production.

## Getting Started

To run the app locally in development mode:

1. Clone the repository and navigate to the project directory
2. Run `docker-compose -f docker-compose-dev.yml up`
3. The app should be available at `http://localhost:3000`

To build and run the app in production:

1. Run `docker-compose up -d --build`
2. The app should be available at `http://localhost`

## Deployment

The app is set up to be deployed to AWS Elastic Beanstalk using GitHub Actions. To deploy the app, push to the `main` branch and the `deploy` workflow will be triggered.

## Built With

- [React](https://reactjs.org/) - JavaScript library for building user interfaces
- [Docker](https://www.docker.com/) - Containerization platform for deploying applications in a consistent environment
- [AWS Elastic Beanstalk](https://aws.amazon.com/elasticbeanstalk/) - Platform for deploying and scaling web applications and services
