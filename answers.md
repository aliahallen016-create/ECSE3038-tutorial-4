POST probe number 1
Status code: 201
number of devices:5

POST probe number 2 
Status code: 201
number of devices: 6

GET probe again 
Status code: 200
number of devices:6

PUT attic 
Status code: 200
number of devices: 6

PUT attic again
Status code: 200
number of devices: 6

DELETE fridge 
status code: 200 
number of devices:5

DELETE fridge again
status code: 404 
number of devices: 5

The PUT and delete request left the system in the same state when I sent the request twice while the POST request did not. This is why the PUT request is idempotent 