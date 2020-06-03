Client side API keys security.

The standard practice is to keep the API keys business on server side to avoid the api key secure.

Problem statement -

But in cases like using map services from google maps OR mapbox the application OR Api keys needs to be attached to the api to get the map rendered on client side. so now the key is visible in browser source code.

This key can be used to access the map service configured.

Solution -
Referer tag & URL restriction.

This project demonstrate the how the exposed token is secured with the Referer tag & URL restriction.

1. The javascript token visible in source code. the hacker can copy the token and use it for accessing the map service. 
![image](https://user-images.githubusercontent.com/8684384/83685080-0bdec080-a5b6-11ea-9944-870cd4c11fd5.png)


2. Access Token copied from the webpage source code and used to run local machine - 
==> The token worked successfully without any issue. (you are hacked !!).

![image](https://user-images.githubusercontent.com/8684384/83685393-97585180-a5b6-11ea-9d57-c76d700b1870.png)


3. To secure the token: let's go the map service provider website and add the url restrictions. 
 
 ![image](https://user-images.githubusercontent.com/8684384/83685803-3b41fd00-a5b7-11ea-94e2-4e59785383db.png)
 
4. Now let's try to access the map service with copied token. 
 
 ![image](https://user-images.githubusercontent.com/8684384/83686647-91fc0680-a5b8-11ea-9f70-492c5b5e58d9.png)
 
 The access token is of no use now !! 
 also check Referer info - https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Referer
