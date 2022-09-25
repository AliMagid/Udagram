# Udacity

## _The trusted market leader in talent transformation_

[![N|Solid](https://www.udacity.com/images/svgs/udacity-tt-logo.svg)](https://www.udacity.com/)

[![License](https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge)](https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt)

# About

### Monolith to Microservices Project

Udagram is a simple cloud application developed alongside the Udacity Cloud Engineering Nanodegree. It allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice.

The project is split into four parts:

1. [Backend RestApi Feed](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/tree/main/udagram-api-feed)
   A a Node-Express server deployed to the cloud to provide the gallery module.
2. [The RestAPI User](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/tree/main/udagram-api-user), A Node-Express server deployed to the cloud to provide the membership module.
3. [Reverseproxy (Api gateway)](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/tree/main/udagram-reverseproxy), A reverse proxy is a server that sits in front of web servers and forwards client (e.g. web browser) requests to those web servers.
4. [Frontend (Ionic App)](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/tree/main/udagram-frontend), The UI app client that integrate with backend RestApi.

# Screenshots

To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline

- DockerHub showing containers that I have pushed
  ![docker-hub](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/DockerHub.png)

- Travis
  ![travis-repo](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/Travis.png)

- Travis CI showing a successful build and deploy job
  ![travis-build-logs](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/TravisBuildLog.png)

## Kubernetes

- To verify Kubernetes pods are deployed properly
  ![running-pods](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/RunningPods.png)

- To verify Kubernetes services are properly set up
  ![running-services-desc](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/K8sGetServices.png)
  ![running-services-desc-p0](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/RunningServicesDescription-0.jpg)
  ![running-services-desc-p1](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/RunningServicesDescription-1.jpg)
  ![running-services-desc-p2](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/RunningServicesDescription-2.jpg)
  ![running-services-desc-p3](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/RunningServicesDescription-3.jpg)

- To verify that you have horizontal scaling set against CPU usage
  ![auto-scale-desc](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/K8sDescribe-hpa.png)

- API pod logs indicates user activity that is logged when an API call is made
  ![login-user-logs](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/LogsIndicatesUserActivity.png)

- To verify that you have set up logging with a backend application K8sDescribe-reverseproxy
  ![reverseproxy-desc](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/K8sDescribe-reverseproxy.png)
  ![reverseproxy-logs](https://github.com/mohammedfarag/udacity-cd0354-monolith-to-microservices-project/blob/main/screenshots/ReversproxyLogs.png)

## URLs:

1. [Frontend-APP](http://ad58295ca6c214889bda880ece0d23dd-384654005.us-east-1.elb.amazonaws.com)
   Link to frontend Ionic app.
2. [Reverseproxy-Gateway](http://a2ea3cca546a14f7397e56778c68c3a2-1644748446.us-east-1.elb.amazonaws.com:8080/api/v0/feed), Link to reverseproxy gateway with port and call for /feed for testing sake.
