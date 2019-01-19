#  Software Engineer(Backend) Challenge

## Background

Here in SETUP TECH, we are developing a platform for real-time data update to end users. As a software engineer in SETUP TECH, you have to provide a reliable backend system and complete web application to clients. Your task here is to develop a web application so as to end users can chat directly in real-time and to implement three endpoints for Custom Mobile App to login the system, to send a message and load/get old message list for a target user.

## Technical Requirement

1. We value a clean, simple working solution.
2. You must provide a `start.sh` bash script at the root of the project, which should setup all relevant applications. It must work on Linux, MacOS.
3. We prefer the following language/platform: `PHP`, `Node.js`.
4. A Database must be used (at SETUP TECH we use mostly MySQL) but PostgreSQL is strongly requested for the challenge. The DB installation & initialisation must be done in `start.sh`.
5. You must submit the project as a git repository (github.com, bitbucket.com, gitlab.com). Repository must avoid containing words `setuptech`, `setuptechchallenge` and `challenge` if it's a public repo.
6. Having unit/integration tests is a strong bonus.
7. Code should be modular, each module should focus on doing one thing and do it well.
8. The solution must be production ready.
9. Avoid over-engineering.

## Challenge Specification

###  Web Application 

1. User friendly Interface will be bonus

2. End user will see the active users who are using the system right now

3. They can send/receive message in real-time

4. Synchronisation with Mobile Application Backend system. 

### API Endpoints

1. Must be a RESTful HTTP API listening to port 8080

2. The API must implement 3 endpoints with path, method, request and response body as specified
  
   - One endpoint to login (see sample)
      * To login, the API client must provide his info
      * The API response is an object containing the active users in system right now
 
   - One endpoint to send a text message (see sample)

     * API responds with a success message

   - One endpoint to list/load all message (see sample)

3. All responses should be in json format no matter in success or failure situations.

# Api interface example

**Login**

* Method: POST

* URL path: /login

* Request body:
  
   ```
   {
  "email": "example@email.com",
  "password": "12345678"
   }
   ```


* Response:

  Header: `HTTP 200` Body:

  ```
  {
   [
    {
     "name":"Full Name",
     "email":"example@email.com"
    },
    {
     "name":"Full Name",
     "email":"example@email.com"
    }
    .
    .
    .
    .
    .
   ]
  }
  ```
  or

  Header: HTTP <HTTP_CODE> Body:

  ```
    {
    "error": "ERROR_DESCRIPTION"
    }
  ```