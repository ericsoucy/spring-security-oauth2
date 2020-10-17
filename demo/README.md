# Based on
<https://spring.io/guides/tutorials/spring-boot-oauth2/>

It uses the authorization code grant to obtain an access token from GitHub (the Authorization Server).


It then uses the access token to ask GitHub for some personal details (only what you permitted it to do), including your login ID and your name. In this phase, GitHub is acting as a Resource Server, decoding the token that you send and checking if it gives the app permission to access the user’s details. If that process is successful, the app inserts the user details into the Spring Security context so that you are authenticated.