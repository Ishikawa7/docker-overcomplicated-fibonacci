# docker-overcomplicated-fibonacci

GENERAL STRUCTURE (components)

Nginx: routing

React: client

Express: server

Worker: to calculate fibonacci number

Redis: to save calculated values

Postgres: to save indicies already seen

FLOW

1)Push code to github

2)Travis automatically pulls repo

3)Travis builds a test image, test code

4)Travis builds prod. image

5)Travis pushes build prod. images to Docker Hub

6)Travis pushes project to AWS Elasticbeanstalk

7)Elasticbeanstalk pulls images from Docker Hub, deploys

