
# -average-alarm-4307
![logo](https://user-images.githubusercontent.com/82109628/208609308-a7f0e4a3-4450-48bf-a094-427f818b1482.png)
<a href="https://github.com/krishna8464/-average-alarm-4307">live</a>
Mailtrap.io![img__homepage-964x574](https://user-images.githubusercontent.com/82109628/208608940-e2f0b84e-0996-41d1-866b-20e44a597903.png)

Team Worked -->>
Team lead   : Yenda Vamshi Krishna(fw22_0324),
Team member : Yuvraj Maharshi(fw22_0817),
Team member : Vivek Mohan Singh(fw22_0596),
Team member : Dhanashri Ahire(fw22_0410).

#To Run
in powershell
-> Set-ExecutionPolicy RemoteSigned
-> Get ExecutionPolicy

#In Terminal
-> json-server --watch db.json


Mailtrap API V1 DocumentationINTRODUCTION⚠ Heads-up! API V2 is outUse API V2 for your new integrationsAPI V1 would be eventually deprecated (no specific date as for October 13, 2022)Mailtrap API is based on the REST principles. The following documentation covers core resources that are used to manipulate the main entities. To start using the Mailtrap API, only a Mailtrap account is required. You have to be authenticated and call the simple HTTPS request on the URL specified below. Please read these basic instructions before you start working with the API.There are several ways to send authenticated HTTP requests:Send a HTTP header Api-Token: {api_token}, where {api_token} is your API tokenSend a parameter api_token={api_token}, where {api_token} is your API tokenSend a HTTP header Authorization: Token token={api_token}, where {api_token} is your API token (more info: Token Access Authentication)Send a HTTP header Authorization: Bearer {jwt_token}, where {jwt_token} is your JWT token (more info: JSON Web Token (JWT))You can find your API/JWT token on your profile page or on the API page in the Mailtrap web application. Both tokens do not have expiration date. You may reset them manually.Allowed HTTPs requests include:POST - to create a resourcePATCH - to update a resourceGET - to get a resource or a list of resourcesDELETE - to delete a resourceHere is the description of common server responses:200 OK - the request was successful (some API calls may return 201 instead).201 Created - the request was successful and a resource was created.204 No Content - the request was successful but there is no representation to return (i.e. the response is empty).400 Bad Request - the request could not be understood or was missing required parameters.401 Unauthorized - authentication failed or user doesn't have permissions for requested operation.403 Forbidden - access denied.404 Not Found - resource was not found.405 Method Not Allowed - requested method is not supported for resource.406 Not Acceptable - the target resource does not have a current representation that would be acceptable to the user agent, according to the proactive negotiation header fields received in the request.409 Conflict - request could not be completed due to a conflict with the current state of the target resource.422 Unprocessable Entity - requested data contain invalid values.429 Too Many Requests - exceeded Mailtrap API limits. Pause requests, wait up to one minute, and try again (you can check rate limits in X-RATELIMIT-LIMIT and X-RATELIMIT-REMAINING headers).API provides JSON and XML request and response. It can be set by:.json or .xml in the end or urlAccept and Content-Type headersAll requests must be sent over HTTPS protocol.![login-fb2fcb15feb36d8e9356](https://user-images.githubusercontent.com/82109628/208609149-5a1707dc-634a-401d-b885-f62b948294df.svg)

REFERENCEUserThis is a section of resources related to the user.![Screenshot_20221220_132915](https://user-images.githubusercontent.com/82109628/208614121-1e1da992-eea7-428e-93d4-9e41d9e46e29.png)

/api/v1/user![Screenshot_20221220_133011](https://user-images.githubusercontent.com/82109628/208614283-c885bc3a-fd85-4ede-9f1d-4969b23548de.png)

GET
This resource does not have any attributes.![Screenshot_20221220_133136](https://user-images.githubusercontent.com/82109628/208614785-52e4eba6-e6ad-4dcc-a2d2-76006c971c66.png)

PATCH
Update user information/api/v1/user/reset_api_token
PATCH![Screenshot_20221220_133228](https://user-images.githubusercontent.com/82109628/208614805-2ed3e020-ce18-47c7-a056-49d884d1c433.png)

Reset user API token
ProjectThis is a section of resources related to the project (company).
/api/v1/companies
GET![Screenshot_20221220_133241](https://user-images.githubusercontent.com/82109628/208614833-73c4493d-0a58-47c4-b955-7e53e0f39add.png)

Get a list of projects (companies) and inboxes
POST
Create a project (company)/api/v1/companies/id
GET
Get project (company) and inboxes
PATCH
Update project (company)
DELETE
Delete project (company) (only if you are the owner of the project, "is_owner: true")/api/v1/companies/id/inboxes
POST
Create inbox in the project (company)
InboxThis is a section of resources related to the inbox
/api/v1/inboxes
GET
Get a list of inboxes/api/v1/inboxes/id
GET
Get inbox![Screenshot_20221220_133257](https://user-images.githubusercontent.com/82109628/208614863-e18ab1bc-110a-4f18-8bb7-bf1eea7c9270.png)

PATCH
Update inbox
DELETE
Delete inbox/api/v1/inboxes/inbox_id/clean
PATCH
Delete all messages (emails) from inbox/api/v1/inboxes/inbox_id/all_read
PATCH
Mark all messages (emails) as read/api/v1/inboxes/inbox_id/reset_credentials
PATCH
Reset inbox credentials/api/v1/inboxes/inbox_id/reset_email_username
PATCH
Reset inbox email address/api/v1/inboxes/inbox_id/toggle_email_username
PATCH
Enable/disable retrieval of messages in this inbox to the specified email address
Shared InboxThis is a section of resources related to a shared inbox
/api/v1/shared_inboxes
GET
Get list of shared inboxes/api/v1/shared_inboxes/id
DELETE

<hr>
Github link : https://github.com/krishna8464/-average-alarm-4307 <br>
Netlify Deployed Link : https://mailtrap.netlify.app/
