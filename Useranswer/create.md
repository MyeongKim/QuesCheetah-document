###**create_useranswer**


POST - (http://quescheetah.com/v1/useranswer/create)

Make a new useranswer.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id",    // Either question_title and question_id is required.
        'update_num'    : "1",                    // The answer_num of answer
        'unique_user'   : "Unique Id"            // For the distiction between useranswers.
    }

```

**return**
``` 
    {
        'useranswer':  {
                            'update_num' : "1",
                            'unique_user': "Unique Id"
                        }       
    }
```