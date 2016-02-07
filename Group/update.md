###**update_question_group**


PUT - (http://quescheetah.com/v1/groups/{groupId})

Update this group data.

You can update all the question data and answer data that is included from this group.

Only update the data passed by request. (On develop)

**request**
```javascript
    {
        "group_name": "This Group name",
        "questions": {
            "1": {
                "question_title": "Your question title 1",
                "question_text": "Your question text 1",
                "start_dt": "", //optional
                "end_dt": "", //optional
                "is_editable": false, // optional
                "is_private": false // optional
            }
            "2": {
                "question_title": "Your question title 2",
                "question_text": "Your question text 2",
                "start_dt": "", //optional
                "end_dt": "", //optional
                "is_editable": false, // optional
                "is_private": false // optional
            }
            ...
        },
        "answers": {
            // Answers for the first question.
            "1": {
                // First answer of the first question.
                "1": {
                    "question_num": 1,
                    "answer_text": "Answer 1"
                    "answer_num": 1,
                },
                "2": {
                    "question_num": 1,
                    "answer_text": "Answer 2"
                    "answer_num": 2,
                },
                ...
            },
            // Answers for the second question.
            "2": {
                // First answer of the second question.
                "1": {
                    "question_num": 2,
                    "answer_text": "Answer 1"
                    "answer_num": 1,
                },
                "2": {
                    "question_num": 2,
                    "answer_text": "Answer 2"
                    "answer_num": 2,
                },
                ...
            },
        }
    }
```
| Arguments | Value | Description |
| --        | --    |
| api_key | string | The user's own api_key. |
| group_name | string | representative title of all questions.| 
| question_title | string | Title of this question. |
| question_text  | string  | Question text to ask. |
| start_dt | long | Activation time of this question. Default is current time.|
| end_dt | long | End time of this question. Default is 30 days from start date.|
| is_editable | string | Determine whether user can change the pre-answered answer.|
| is_private | string | Show question to added urls only. |
| answer_num | integer | Be criterion of descending order. Lower number will go first.|
| answer_text | string | Giving texts to choose. |


**return**
```javascript
    {
        "questions": [
            {
                "id": 1,
                "is_editable": false,
                "title": "title 1",
                "start_dt": "2016-02-07T14:34:44.873",
                "is_private": false,
                "end_dt": "2016-03-08T14:34:44.873",
                "text": "text 1"
            },
            {
                "id": 2,
                "is_editable": false,
                "title": "title 2",
                "start_dt": "2016-02-07T14:34:44.880",
                "is_private": false,
                "end_dt": "2016-03-08T14:34:44.880",
                "text": "text 2"
            }
        ],
        "group_id": 5,
        "group_name": "myname"
    }
```