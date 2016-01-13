###**to_private**


POST - (http://quescheetah.com/v1/question/private)

Change question state to private.

**request**
```javascript 
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id"    // Either question_title and question_id is required.
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key |
| question_title | string | Title of this question |
| question_id  | integer  | Id of this question |


**return**
```javascript 
    {
        "result": "success",
        "description": "Update description"
    }
```
    
###**to_public**


POST - (http://quescheetah.com/v1/question/public)

Change question state to public.

**request**
```javascript 
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id"    // Either question_title and question_id is required.
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key |
| question_title | string | Title of this question |
| question_id  | integer  | Id of this question |

**return**
```javascript 
    {
        "result": "success",
        "description": "Update description"
    }
```
    
###**get_url_list**


POST - (http://quescheetah.com/v1/question/url/list)

Get authenticated urls of the question.

**request**
```javascript 
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id"    // Either question_title and question_id is required.
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key |
| question_title | string | Title of this question |
| question_id  | integer  | Id of this question |

**return**
```javascript 
    {
        "urls": [
            0: {
                "https://naver.com"
            },
            1: {
                "https://google.com"
            },
            2: {
                "https://daum.net"
            },
            ...
        ]
    }
```
    
###**add_url**


POST - (http://quescheetah.com/v1/question/url/add)

Add an authenticated url.

**request**
```javascript 
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id",    // Either question_title and question_id is required.
        "url"           : "New url"
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key |
| question_title | string | Title of this question |
| question_id  | integer  | Id of this question |
| url | string | New url that user want to add |

**return**
```javascript 
    {
        "urls": [
            0: {
                "https://naver.com"
            },
            1: {
                "https://google.com"
            },
            2: {
                "https://daum.net"
            },
            ...
        ]
    }
```