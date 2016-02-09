# REST API

All request to QuesCheetah are processed with REST API.

You send the request data in JSON format.

you should set ```content-type: application/json``` in the request header.

For the authentication you should always add ```api-key``` to the request header.

Or further secure connection, instead of ```api-key```, you can use your ```jwt``` token value and ```kid```.

###**Request header**
```javascript
curl https://localhost:8000/v1/groups/1 \
    -X GET \
    -H 'content-type: application/json' \
    -H 'api-key: { Your key }'

```

```javascript
curl https://localhost:8000/v1/groups/1 \
    -X GET \
    -H 'content-type: application/json' \
    -H 'jwt: { Your token }' \
    -H 'kid: { Your kid }'

```


The response will be always JSON object.



###**Error response**

```javascript
    {
	    "error": True,
	    "description": "Error description" // this data depends on the context.
    }
```


###**Errors**
| Number | Description |
| -- | -- |
| 200 | OK - Everything went as planned. |
| 400 | Bad Request - Something in your header or request body was malformed. |
| 401 | Unauthorized - Necessary credentials were either missing or invalid. |
| 404	 | Not Found - The object you’re requesting doesn’t exist. |
| 500	 | Server Errors - Something went wrong on our end. |
