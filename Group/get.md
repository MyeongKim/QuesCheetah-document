###**get_question_group**


GET - (http://quescheetah.com/v1/groups/{groupId})

Get this group, question, answer data.


**return**
```javascript
    {
        "group_id": 1,
        "group_name": "myname",
        "question": {
            "question_id": 3,
            "answers": [
                {
                    "answer_count": 1,
                    "answer_num": 1,
                    "answer_text": "mytext1"
                },
                {
                    "answer_count": 1,
                    "answer_num": 2,
                    "answer_text": "mytext2"
                }
            ],
            "question_text": "q_text",
            "question_title": "q_title"
        }
    }
```
