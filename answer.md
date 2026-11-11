#Task 3: Idempotence 
#Observation on Idempotence 

1.POST/devices first trial: status 201, Devices after:5 
2.POST/devices second trial: status 201, Devices after:6
3.PUT/devices/attic first trial: status 200, Devices after: 6 
4.PUT/devices/attic second trial: status 200, Devices after: 6
5.DELETE/devices/fridge first trial: status 200, Devices after: 5 
6.DELETE/devices/fridge first trial: status 404, Devices after: 5 
