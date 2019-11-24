# REST API

## Save Employee:

```
$ curl -H "Content-Type: application/json" -X POST -d '{"name": "Arpit","address": {"city": "Delhi","zipCode": "10098"}}' http://localhost:8000/employee/save
```

## List All

```
$ curl -X GET http://localhost:8000/employee/list/
```


## List One
```
$ curl -X GET http://localhost:8000/employee/list/1
```

# Deploying to Heroku

```
$ heroku create
$ git push heroku master
$ heroku open
```
## Deployment on - https://gentle-lake-06150.herokuapp.com/

# Receive Side

## URL - http://localhost:8000/visa/receive/oct

## Request

```
{
	"encRecipientPAN":"1234567890"

}
```

## Response

```
{
    "responseCode": "00",
    "receiverTransactionId": "00",
    "authIdResponse": "00",
    "cpsAuthorizationCharacteristicsIndicator": "00"
}
```
