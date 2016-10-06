# How to use Swagger UI on IBM Bluemix

## Overview

I wanted to share API specification with my client on swagger and I needed to web server to install swagger UI to access each other.
I found API connect service on Bluemix which support to API management but I don't like UI and I just want to use default swagger UI.
Therefore I tried to set swagger UI on Bluemix using SDK for Node.js.

### How to set up

1. Create the account of IBM Bluemix
2. Add the Cloud Foundry Application for SDK for Node.js
3. Set up the Cloud Foundry Command Line Interface and Bluemix Command Line Interface

	`https://github.com/cloudfoundry/cli/releases
	 http://clis.ng.bluemix.net/ui/home.html`

3. Clone this commit
4. Change `./publish/swagger.json` to your own one
4. Change directory to downloaded directory
5. Connet to IBM Bluemix

	`$bluemix api https://api.{your choosen country domain}.bluemix.net`
6. Login to Bluemix

	`$bluemix login -u {your email address} -o {your grouop name} -s {your space name}`
	
7. Execute the cf push command and wait to finish build and deployment

	`$cf push`
	
8. Access by web browser to 
	`http://{yourdomain}.mybluemix.net`

9. #####Swagger UI will open!!
