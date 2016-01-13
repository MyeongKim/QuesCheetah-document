###**simple_view_answer**


POST - (http://quescheetah.com/v1/answer/view/simple)

Provide the main information of question.

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
        "question_title": "Your question title",
        "question_text": "Your question text",
        "answer": [{
            "answer_num": "1",
            "answer_text": "answer1",
            // 'answer_count' means how many useranswers are made with this answer. 
            "answer_count": 2
        }, {
            "answer_num": "2",
            "answer_text": "answer2",
            "answer_count": 4
        }, {
            "answer_num": "3",
            "answer_text": "answer3",
            "answer_count": 1
        }, {
            "answer_num": "4",
            "answer_text": "answer4",
            "answer_count": 2
        }]
    }
```