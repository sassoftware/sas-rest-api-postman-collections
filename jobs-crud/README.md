This collection performs CRUD operations on a job. First, it creates a job definition which runs a simple print statement in SAS code. Next it executes the job. Followed by a check for the job and verification of the job state. In the final step, the job definition is deleted. 

### Authentication
For more info on registering clients and Authentication, please see the [Configuring Your SAS Environment for API Use](https://developer.sas.com/apis/rest/Topics/#configuring-your-sas-environment-for-api-use) and [Authentication and Access Tokens](https://developer.sas.com/apis/rest/Topics/#authentication-and-access-tokens) on [developer.sas.com](https://developer.sas.com/home.html), or read the [Authentication to SAS Viya: a couple of approaches](https://blogs.sas.com/content/sgf/2019/01/25/authentication-to-sas-viya/) blog post. 

The first API call contains a Pre-requisite script to obtain an access token. See Postman Pre-requisites for more information about required environment variables. If you wish to authenticate in another manner, feel free to adjust the calls as needed.

### Postman Pre-requisites
* Create an environment with the following variables:
    * encoded_id_secret - base64 encoded value of client_id:client_secret
    * OAUTH_USERNAME - SAS username
    * OAUTH_PASSWORD - SAS password
    * sasserver - name of the SAS server formatted for connection i.e., https://mysasserver.sas.com