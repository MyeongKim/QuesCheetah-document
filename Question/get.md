###**get_question**


GET - (http://quescheetah.com/v1/questions/{questionId})

Get question data. Return json includes question and answer data.


**return**
```javascript 
    {
        "questions": {
            "1": {
                "id": "question id",
                "question_title": "Your question title 1",
                "question_text": "Your question text 1",
                "start_dt": "2016-02-09T04:57:15.322",
                "end_dt": "2016-02-09T04:57:15.322",
                "is_editable": { false },
                "is_private": { false }
            }
        },
        "answers": {
            "1": {
                // First answer of the first question.
                "1": {
                    "id": "answer id",
                    "answer_count": "answer count",
                    "answer_text": "Answer 1"
                },
                "2": {
                    "id": "answer id",
                    "answer_count": "answer count",
                    "answer_text": "Answer 2"
                }
            }
        }
    }
```


###**get_simple_result**


GET - (http://quescheetah.com/v1/questions/{questionId}/SimpleResult)

Get only important data of this question.


**return**
```javascript 
    {   
        "id": "question id",
        "question_text": "Your question text",
        "question_title": "Your question title",
        "answers": [
            {
                "id": "answer id",
                "answer_text": "My answer text for two",
                "answer_count": 0, // How many users voted to this answer.
                "answer_num": 2 
            },
            {
                "id": "answer id",
                "answer_text": "My answer text for one",
                "answer_count": 0, // How many users voted to this answer.
                "answer_num": 1
            }
        ]
    }
```