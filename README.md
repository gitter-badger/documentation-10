# Citizen Science Center

## Who?

We are a Competence Center that is joint with UZH and ETH in Switzerland. The goal of the center is to develop and utilise existing crowd sourcing tools to enable researchers to access the power of the crowd.

## How?

This is being done by developing an easy-to-use crowd-sourcing project tool that enables users \(both technical and otherwise\) to create projects with a variety of requirements.

## What?

C3S is a platform created to connect researchers with citizen scientists by allowing them to create custom apps without a requirement of technical experience. The flexibility of the platform allows researchers to create apps for mobile and web and share them with the world. Apps created through the platform can be publicised within the community and data can be queried and accessed.

## Structure

`Projects` are made up of `tasks`, users can participate in a task by adding `submissions`. A task consists of a question and an answer, some examples could be:
* Recording mood every day
* Uploading a geolocated image
* Multiple choice
* Select from a grid of images (or tweets, videos etc)

## Technical Stuff

Using Postgres as the backend database allows for a basic fixed structure with the flexibility of JSON storage in select fields, giving the benefits of relational with some of the features of NoSQL. The API is powered by the OpenAPI standard and can be accessed in YAML or JSON form. Using the standard allows tools to be easily created and ensures the endpoints are well documented.

