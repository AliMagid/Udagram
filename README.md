# Udacity

## _The trusted market leader in talent transformation_

[![N|Solid](https://www.udacity.com/images/svgs/udacity-tt-logo.svg)](https://www.udacity.com/)

[![License](https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge)](https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt)

# About

### Monolith to Microservices Project

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into four parts:

1. [Backend RestApi Feed](https://github.com/AliMagid/Udagram/tree/main/udagram-api-feed)
   A a Node-Express server deployed to the cloud to provide the gallery module.
2. [The RestAPI User](https://github.com/AliMagid/Udagram/tree/main/udagram-api-user), A Node-Express server deployed to the cloud to provide the membership module.
3. [Reverseproxy (Api gateway)](https://github.com/AliMagid/Udagram/tree/main/udagram-reverseproxy), A reverse proxy is a server that sits in front of web servers and forwards client (e.g. web browser) requests to those web servers.
4. [Frontend (Ionic App)](https://github.com/AliMagid/Udagram/tree/main/udagram-frontend), The UI app client that integrate with backend RestApi.

# Screenshots

## Deployment Pipeline

- DockerHub showing containers that I have pushed
  ![docker-hub](https://github.com/AliMagid/Udagram/blob/main/screenshots/Dockerhub.jpg)

- Travis CI showing a successful build and deploy job
  ![travis-build-logs](https://github.com/AliMagid/Udagram/blob/main/screenshots/Travis.png)

## Kubernetes

- To verify Kubernetes pods are deployed properly
  ![running-pods](https://github.com/AliMagid/Udagram/blob/main/screenshots/get%20pods.png)

- To verify Kubernetes services are properly set up
  ![running-services-desc](https://github.com/AliMagid/Udagram/blob/main/screenshots/get_services.png)
  ![running-services-desc-1](https://github.com/AliMagid/Udagram/blob/main/screenshots/descrive_services_1.png)
  ![running-services-desc-2](https://github.com/AliMagid/Udagram/blob/main/screenshots/describe_services_2.png)
  ![running-services-desc-3](https://github.com/AliMagid/Udagram/blob/main/screenshots/describe_services_3.png)
  ![running-services-desc-4](https://github.com/AliMagid/Udagram/blob/main/screenshots/describe_services_4.png)

- To verify that you have horizontal scaling set against CPU usage
  ![auto-scale-desc](https://github.com/AliMagid/Udagram/blob/main/screenshots/hpa.png)

- API pod logs indicates user activity that is logged when an API call is made
  ![login-user-logs](https://github.com/AliMagid/Udagram/blob/main/screenshots/get_logs.png)


## URLs:

1. [Frontend-APP](http://a0b5e4e2774d84d5fbe5019df192514e-885545366.us-east-2.elb.amazonaws.com)
   Link to frontend Ionic app.
2. [Reverseproxy-Gateway](http://a3daf0ffa0c9b4eb88e868f32fe36561-985664241.us-east-2.elb.amazonaws.com:8080/api/v0/feed), Link to reverseproxy gateway with port and call for /feed for testing sake.
