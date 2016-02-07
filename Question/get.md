###**get_question**


GET - (http://quescheetah.com/v1/questions/{questionId})

Get question data. Return json includes question and answer data.


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


###**get_simple_result**


GET - (http://quescheetah.com/v1/questions/{questionId}/SimpleResult)

Get only important data of this question.


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