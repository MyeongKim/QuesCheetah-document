###**get_question**


POST - (http://quescheetah.com/v1/question/get)

Get question data. Not related answers.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id",    // Either question_title and question_id is required.
    }

```

**return**
``` 
    {
        'api_key'           : "Your api key",
        'question_title'    : "Your question title",
        'question_text'     : "Your question text",
        'start_dt'          : "",                   
        'end_dt'            : "",                   
        'is_editable'       : "True",               
        'is_private'        : "True",           
    }
```