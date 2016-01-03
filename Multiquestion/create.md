###**create_multiple_question**


POST - (http://quescheetah.com/v1/multiple/create)

Create many question.

These questions are grouped together.

The answers within each question are created also.

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
                            2: {
                                    'question_title': "Your question title 2",
                                    'question_text' : "Your question text 2",
                                    'start_dt'      : "",       //optional
                                    'end_dt'        : "",       //optional
                                    'is_editable'   : "True",   // optional
                                    'is_private'    : "True"    // optional
                                    }
                                    
                            ...        
                            
                           }
        'answers'     : {
                            // Answers for the first question.
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
                            // Answers for the second question.
                            2:  {   
                                    // First answer of the second question.
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
        'multiquestion' :   {
                                'group_name':   "Your group name"
                            },
        'questions'      :   {
                                0:  {
                                        'question_title': "Your question title",
                                        'question_text': "Your question text"
                                    },
                                1:  {
                                        'question_title': "Your question title",
                                        'question_text': "Your question text"
                                    }
                                
                                ...
                                
                            }
        
    }
```