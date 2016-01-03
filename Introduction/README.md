# REST API

All request to QuesCheetah are processed with REST API.

You send the request data in JSON format.

you should set ```content-type: application/json``` in the request header.

The response will be always JSON object. It depends on the context.


###**Error response**

```javascript
    {
	    "error": boolean,
	    "description": string // this data depends on the context.
    }
```