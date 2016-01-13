###**create_question**


POST - (http://quescheetah.com/v1/question/create)

Create one question. Not any related answers.

**request**
```javascript 
    {
        "api_key"           : "Your api key",
        "question_title"    : "Your question title",
        "question_text"     : "Your question text",
        "start_dt"          : "",                   // optional
        "end_dt"            : "",                   // optional
        "is_editable"       : "True",               // optional
        "is_private"        : "True",               // optional
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key. |
| question_title | string | Title of this question. |
| question_text  | string  | Question text to ask. |
| start_dt | long | Activation time of this question. Default is current time.|
| end_dt | long | End time of this question. Default is 30 days from start date.|



**return**
```javascript 
    {
        "api_key"           : "Your api key",
        "question_title"    : "Your question title",
        "question_text"     : "Your question text",
        "start_dt"          : "",                   
        "end_dt"            : "",                   
        "is_editable"       : "True",               
        "is_private"        : "True",               
    }
```