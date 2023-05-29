# SushiCo
Sushi Based API

Problem Statement

NewCo is a new company and is in need of a way to collect all the sushi
restaurants in a particular city. They would like to be able to query some
software by sending it a city name within the USA. The software should
send back a list of all sushi restaurants in the city. If there are no sushi
restaurants in the city it should send back an empty list and a status that
no sushi restaurants were found.

Solution Statement

Develop a software web service that has a request protocol to query
established 3rd party internet services (i.e. Google Maps, etc.) to ingest,
aggregate and form the restaurant list.

'''
NOTES:
'''

INITIAL THOUGHTS:
swagger api (use to build the bridge connection between the client and ser ver {aka the sushi}) -> postman (validation) -> then create a web using python and fastapi (python) 

^^ 
Create FASTAPI First
Use Swagger to Document The Framework so its more readable
Postman to check everytjing


YELP API (no location coords required)
- required params:
  - location
  - term (keyword)
  - radius
make sure the keyword is automatically sushi
keep simple
connect requests to API endpoint (get)

i think return {
     response.json()
}
is how u do it but im not too sure

- learn how to authorize
- learn the difference between user/business/client id and the authorization key
 


uploading everything onto github

400 : BAD REQUEST
404: NOT FOUND
200: ok aka go on  with the code (successfull requestion)

200 OK
General success status code. This is the most common code. Used to indicate success.
201 CREATED
Successful creation occurred (via either POST or PUT). Set the Location header to contain a link to the newly-created resource (on POST). Response body content may or may not be present.
204 NO CONTENT
Indicates success but nothing is in the response body, often used for DELETE and PUT operations.
400 BAD REQUEST
General error for when fulfilling the request would cause an invalid state. Domain validation errors, missing data, etc. are some examples.
401 UNAUTHORIZED


After everything, I learnt that the project was much more simplistic in terms of coding and requests. Furthering onwards I can advance this simple API into a web service using HTML and CSS.

