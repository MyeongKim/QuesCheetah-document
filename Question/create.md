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