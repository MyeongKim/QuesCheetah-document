###**get_question_group**


GET - (http://quescheetah.com/v1/groups/{groupId})

Get this group, question, answer data.


**return**
```javascript
    {
        "group_id": "This Group id",
        "group_name": "This Group name",
        "questions": {
            "1": {
                "question_title": "Your question title 1",
                "question_text": "Your question text 1",
                "start_dt": "2016-02-09T04:57:15.322",
                "end_dt": "2016-02-09T04:57:15.322",
                "is_editable": { false },
                "is_private": { false }
            }
            "2": {
                "question_title": "Your question title 2",
                "question_text": "Your question text 2",
                "start_dt": "2016-02-09T04:57:15.322",
                "end_dt": "2016-02-09T04:57:15.322",
                "is_editable": { false },
                "is_private": { false }
            }
            ...
        },
        "answers": {
            // Answers for the first question.
            "1": {
                // First answer of the first question.
                "1": {
                    "answer_text": "Answer 1"
                },
                "2": {
                    "answer_text": "Answer 2"
                },
                ...
            },
            // Answers for the second question.
            "2": {
                // First answer of the second question.
                "1": {
                    "answer_text": "Answer 1"
                },
                "2": {
                    "answer_text": "Answer 2"
                },
                ...
            },
        }
    }
```
