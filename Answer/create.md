###**create_answer**


POST - (http://quescheetah.com/v1/answer/create)

Create answers related to one question.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id",    // Either question_title and question_id is required.
        'answers': {
                        1:{'answer_num':"1", 'answer_text': "answer1"},
                        2:{'answer_num':"2", 'answer_text': "answer2"},
                        3:{'answer_num':"3", 'answer_text': "answer3"},
                        4:{'answer_num':"4", 'answer_text': "answer4"}
                    }
    }

```

**return**
``` 
    {
        'answers': {
                        1:{'answer_num':"1", 'answer_text': "answer1"},
                        2:{'answer_num':"2", 'answer_text': "answer2"},
                        3:{'answer_num':"3", 'answer_text': "answer3"},
                        4:{'answer_num':"4", 'answer_text': "answer4"}
                    }             
    }
```