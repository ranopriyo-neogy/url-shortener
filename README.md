# Overview

This is a url shortner service that takes a long url from the user and make it short. The backend used for this service is MongoDB Atlas. The service takes two types of request. The first request is generating the short url based on long url input and stores it in MongoDB database. The second request is for routing the short url to the associated long url stored in the database.

## How to use

- Clone the repository using `git clone https://github.com/ranopriyo-neogy/url-shortener.git`
- Get into the project folder using `cd url-shortener`
- Make sure you have docker installed and running in your system. 
- Run `docker-compose up`
- From any REST Client hit - `http://localhost:5000/api/url/shorten` with `POST` operation and pass a long url in below JSON format:
```
{
    "longUrl": "Enter your long URL Here"
}
```
- The Response will be having the short url.
- Then we can try hitting the short url and it will route us to the associated long url.

## Request and Response - REST Client

![](./architecture/rest_client.png)

## High Level Service Architecture

![](./architecture/Highlevel.png)

## Detailed Service Architecture

![](./architecture/detailed_arch.png)

## Backend Database - MongoDB 

For testing purpose I have provided my application connection string in this project for connecting to the backend DB. However to build this from scratch one has to create an account in https://account.mongodb.com/account/login and define a cluster and connect using their respective Application connection string.

![](./architecture/MongoDB.png)

### MongoDB cost

![](./architecture/mongodb_cost.png)

## Developer

- [Ranopriyo Neogy](https://github.com/ranopriyo-neogy)
