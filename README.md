# Authentication_ASP.NET
This project was to create an authentication system using localdb and twitter OAuth to create and store users. In this project I also created user roles and assigned them to existing users (manually) so they could access certain pages.

## how to run
initially twitter OAuth won't work as it requires your API public and secret key, to make this work you have to:

1. go to [apps.twitter.com](https://apps.twitter.com/)  
1. create an account then create a project  
1. when creating the project fill out the required fields  
1. on the website field enter: ` https://127.0.0.1:44348 ` make sure the port is correct for your URL when you launch the website through visual studio  
1. in the callback URLs make sure you have there 2 links with the correct ports ` https://localhost:44348/signin-twitter ` and ` https://localhost:44348 ` in the field  
1. select ` Allow this application to be used to Sign in with Twitter ` radio button  
1. finish creating.  
1. go to the tab ` Keys and Access Tokens `  
1. copy consumer Key/Secret and copy paste them inside the `Startup.Auth.cs` file in `Authentication/App_Start/Startup.Auth.cs` on line 61 and 62 in place of the 'xxxx'  

