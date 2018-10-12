# ResponseToFile-Postman

This project will help in writing the responses of a request from Postman

This project is to be used with template from Postman.

### Steps to install the template
1. Launch Postman Native App [Download Postman](https://getpostman.com/apps)
2. Visit the following URL: https://documenter.getpostman.com/view/3407886/RWgp1fB5
3. Click `► Run In Postman` and open with the native app

The collection that was imported makes it easy for users who want to write the response of each request to a file.
This can be extended to write anything for eg. meta information or value of variables being used.

PR's are welcome.

----
_Collection Docs:_

This project is using a powerful feature built in postman called as `pm.sendRequest`, the docs for which can be found here: https://www.getpostman.com/docs/v6/postman/scripts/postman_sandbox_api_reference


### Requirements
To work with this script, a local server is required.
You can choose to write your own local server or edit the one provided below as per your needs.

### Steps To Use
1. Put all the requests you want to write the responses for, under this collection.
 
2. Clone the following repository to your machine - https://github.com/sivcan/ResponseToFile-Postman or use the following command - `git clone https://github.com/sivcan/ResponseToFile-Postman`

3. Navigate into the directory and install the dependencies. Use the following command: `npm i` 

4. Run the local server. Use the following command: `node script.js`

5. Now, the responses for every request which is a part of this collection will be written to the `Responses` folder inside the project repo.
You can modify the local server's code to change the file location.

5. Run your requests through builder / run through collection runner and store your data locally. 


Currently, this supports only writing JSON data.
You can modify the script and the local server to support CSV or other formats of data as per your needs.

### Additionally
Instead of moving each request under this collection, you can copy the script from the `Tests` tab of this collection to the `Tests` tab of any request or even a specific folder.
On running that particular request / folder, it'll work.