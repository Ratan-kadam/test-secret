Client side API keys security.

The standard practice is to keep the API keys business on server side to avoid the api key secure.

Problem statement -

But in cases like using map services from google maps OR mapbox the application OR Api keys needs to be attached to the api to get the map rendered on client side. so now the key is visible in browser source code.

This key can be used to access the map service configured.

Solution -
Referer tag & URL restriction.

This project demonstrate the how the exposed token is secured with the Referer tag & URL restriction.
