# SSP Technical Interview

### About

This is the "server" portion of the technical interview. The intent of this application 
is for the applicant to create a "client" application which will call this app's
getCustomerVehicle API to retrieve a customer's vehicle information by
the customer's id (all mocked data).

 >Server port is set to `9091` to avoid conflicts with other applications

### User Story

* See word document attached here (Interview_User_Story.docx) which includes the same 
information as below plus a Swagger screenshot of the API the applicant is to integrate
with 

#### Task
As a Subscription Services Platform consumer \
I want to retrieve a customer's vehicle information by their customer id \
So that I can see information about the vehicle that belongs to the customer

#### Acceptance Criteria
Return only the vehicle information with the contract of:
```
vin : string
year : int
model : string
```

#### Notes
* A customer will have only 1 vehicle associated with their id
* Customer vehicle information can be retrieved from:
  * http://localhost:9091/customer/{id}