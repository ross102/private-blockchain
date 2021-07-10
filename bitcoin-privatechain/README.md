# Starting the application

1. Cd into project_1_V2_boilerplate directory.
2. Run `npm install` to install the required packages
3. After installing the packages, run `node app.js` to start the project.
   You should see server running on port 8080 in the terminal


## Understanding the project structure

The Boilerplate code is a simple architecture for a Blockchain application, it includes a REST APIs application to expose the your Blockchain application methods to your client applications or users.

1. `app.js` file. It contains the configuration and initialization of the REST Api.
2. `BlockchainController.js` file. It contains the routes of the REST Api. Those are the methods that expose the urls you will need to call when make a request to the application.
3. `src` folder. In here we are going to have the two main classes we needed to create our Blockchain application.


## Making Requests

1. Run the application using the command `node app.js`
You should see in your terminal a message indicating that the server is listening in port 8000:
> Server Listening for port: 8000

2. Creating the Genesis block:
     `http://localhost:8000/block/height/0` 
3. Retrieve blocks by hash
     `http://localhost:8000/blocks/hash/<HASH>`
4. Make your first request of ownership sending your wallet address:
    `http://localhost:8000/requestValidation `
5. Submit your Star
      `http://localhost:8000/submitstar`
6. Retrieve Stars owned by me
     `http://localhost:8000/blocks/<WALLET_ADDRESS>`

