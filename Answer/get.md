###**get_answer**


POST - (http://quescheetah.com/v1/answer/get)

Get all answer data related with one question.

**request**
```javascript 
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id",    // Either question_title and question_id is required.
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string | The user's own api_key. |
| question_title | string | Title of this question. |
| question_id  | integer  | Id of this question. |

**return**
```javascript 
    {
        "answers": [
            1: {
                "answer_num": "1",
                "answer_text": "answer1"
            },
            2: {
                "answer_num": "2",
                "answer_text": "answer2"
            },
            3: {
                "answer_num": "3",
                "answer_text": "answer3"
            },
            4: {
                "answer_num": "4",
                "answer_text": "answer4"
            }
        ]
    }
```