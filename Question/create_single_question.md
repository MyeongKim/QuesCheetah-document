###**create_single_question**


POST - (http://quescheetah.com/v1/single/create)

Create single question.
The answers of the question are created also.

**request**
```
    {
        'api_key'       : "Your api key",
        'group_name'    : "This Group name",
        'questions'     : {
                            1: {
                                    'question_title': "Your question title 1",
                                    'question_text' : "Your question text 1",
                                    'start_dt'      : "",       //optional
                                    'end_dt'        : "",       //optional
                                    'is_editable'   : "True",   // optional
                                    'is_private'    : "True"    // optional
                                    }       
                           }
        'answers'     : {
                            1:  {   
                                    // First answer of the first question.
                                    1:  {
                                            'answer_num': "1",
                                            'answer_text' : "Answer 1"
                                        },
                                    2:  {
                                            'answer_num': "2",
                                            'answer_text' : "Answer 2"
                                    },
                                    
                                    ...
                                    
                                    
                                },
                           }
    }

```

**return**
```
    {   
        
        
    }
```
