# Kyle Felter

kylerfelter@gmail.com

[github.com/kfelter](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter)

## Projects
* [ref collector](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/ref_collector) - collects visits on my various projects and writes data about the visit to postgres
* [react/python/serverless](https://kfelter.com/?ref=gh_profile&dst=http://hueput.kfelter.com) - color picking and voting app deployed using aws s3 and aws lambda
* [recursive forest generation](http://kfelter.com/?ref=gh_profile&dst=http://forest.kfelter.com) - fun project that uses javascript to recursively generate a forest
* [gRPC example](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/grpc-example) - simple grpc NoSQL database client and server using golang
* [protobuf example](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/protobuf-example) - simple example demonstrating how to use protobuf in golang
* [tolerance](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/tolerance) - fault tolerant math operations in golang inspired by spacex
* [apguard](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/apguard) - distributed proxy that acts as a rate limiter for downstream http services
* [c++ arduino game](http://kfelter.com/?ref=gh_profile&dst=https://youtu.be/zAuerOaZ_Z8) - memory game deployed on an arduino
* [go concurrecny model](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/go_concurrency_example) - examples of how to use channels and go routines to design concurrent go code
* [Caverunner](http://kfelter.com/?ref=gh_profile&dst=https://filebox.ece.vt.edu/~mhsiao/video_game/proj2016/kyle_felter.html) - While creating this game I had to think about limitations of graphics within the browser and how to make the code efficient enough to run on most computers.
* [Path finding Hokie](http://kfelter.com/?ref=gh_profile&dst=https://filebox.ece.vt.edu/~mhsiao/video_game/proj2016/Proj8_4.html) - fun game that uses BFS to move a Hokie around in a maze.
* [Basketball Game](http://kfelter.com/?ref=gh_profile&dst=https://filebox.ece.vt.edu/~mhsiao/video_game/proj2016/Proj5_4.html) - physics simulation in javascript used to make a small basketball game.
* [things](http://kfelter.com/?ref=gh_profile&dst=https://github.com/kfelter/termpi) (not active)- basic crud app for managing raspberry pi clusters


## Resume
[pdf](/resume.pdf) [MD](/resume.md)

 

# KYLE FELTER

kylerfelter@gmail.com

Alexandria, Virginia 22314

## About

I'm an expert in writing golang solutions for large scale engineering challenges. I've created and maintained large data pipelines, public api's, and background processing jobs. I've also managed infrastructure and service uptimes with monitoring and alerting technologies.

## Skills and Abilities

Golang (5+ years), ClI/CD, Docker And Micro Service Architecture, kubernetes, python, SQL and noSQL databases, cloud native design, minimalistic code orginization (the less there is the less likely there will be a bug), Google Cloud Platform, AWS, Linux

## Employment History

### 01/2021 - Present Engineer II Spotify

Megaphone was purchased by Spotify, my contributions to the adserver and content delivery code around Streaming
Ad Insertion was a large contributor to the deal. I still lead the backend development team that focuses on scaling up
to 1 billion podcast downloads a month and beyond.

Recently I 
* migrated our infrastrucure from on prem machines running rancher to gke in google cloud
* upgraded a large batch job that to an event driven system that improved accuracy, observability, reliability, speed and scaling potential of the system
* created new revenue streams by adding the ability to communicate via the VAST spec to our adserver
* created a new reporting pipeline to track ad impression events for billing purposes
* led code walkthrough's to help other developers understand the business logic of applications

### 09/2019 - 01/2021 Software Engineer Megaphone

Megaphone is a leader in technology supporting podcasts. I am the lead developer on the backend services that
support audio streaming and dynamic advertisement insertion.

Main efforts:

* Migrate audio data services from heroku with a managed cdn to kubernetes on bare metal
* Improve audio delivery architecture using golang/nginx/docker/kubernetes
* Adding features to the advertisement delivery service written in golang
* Setup CI/CD pipelines to automate testing and deployment of code updates
* General software engineering and debugging on a platform with many interacting technologies, including digging into bugs and filtering large data sets to illuminate root causes of a bug effecting multiple parts of a larger system

* Main languages used: golang, python, bash

* Support and mentor junior golang developers through PRs and 1 on 1 meetings

### 11/2018 - 09/2019 Full Stack Developer, Product Decipher Technology Studios

[ Product Development ]

Al machine learning using neural nets to analyze time series data: pytorch
Api integration: REST, go packages, react components

Web service development: react, go

Golang development: encryption, jwt web tokens

[ DevOps ]
Devops CI/CD: openshift, Jenkins, circleci
Micro service architecture and containers: docker

### 07/2017 - 11/2018 Associate Technical Consultant Blackstone Technology Group

[ Product Development ]

REST API development in Golang

UI Design in Angular typescript

AWS service integration: s3, lambda, ec2, iam
Secure access management using jwt and Keycloak

[ DevOps ]

Infrastructure as code: Terraform, Ansible

Highly available / Clustered services: Hashicorp consul, DNS
Automating Auditing and Security scanning: Graylog, Nessus
Linux os hardening: CENTOS, SELinux



## Education History

Virginia Polytechnic Institute and State University 
Bachelor's Degree in Computer Engineering

I started out as an Electrical engineer but found myself writing code to solve most of my homework and exams. This
lead me to change majors into computer engineering, which focuses on creating practical solutions with software to
solve real world problems.

## Personal Projects

### 01/2019 - 02/2019 HuePut 

Https://s3.amazonaws.com/core-color/index.html

* Add new colors to a community board
* Vote on colors by liking them
* Frontend is written in react hosted as static content in AWS s3
* Backend is an AWS lambda function + s3 as a DB

I really enjoyed making this project, I created it in such a way that the server that hosts the content does not exist until
a user interacts with it. As soon as a user visits the site, a server is created, content is served, then the server is
deleted. Every time an action is performed on the site it goes through this process, saving costs on AWS resources
and allowing it to be infinitely scalable.


### 07/2020 - 08/2020 GoTolerance 

This is a golang package that runs math operations in multiple go routines, using parallel processes to run the same
math operation multiple times. Then it compares all the parallel operations and tries to get a majority vote on the
correct answer. This allows us to continue math operations even if one of our processes were corrupted by the
physical environment.

## Certifications & Honors

12/2018 Best Hackathon Project 2018 Decipher Technology
Studios

service that created a graph representing microservice dependencies using http request tracing


## Additional Info

GitHub: kfelter

Projects page: kfelter.github.io

