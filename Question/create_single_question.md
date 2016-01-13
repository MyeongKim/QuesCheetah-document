###**create_single_question**


POST - (http://quescheetah.com/v1/single/create)

Create single question.
The answers of the question are created also.

**request**
```javascript
    {
        "api_key": "Your api key",
        "group_name": "This Group name",
        "questions": [
            1: {
                "question_title": "Your question title 1",
                "question_text": "Your question text 1",
                "start_dt": "", //optional
                "end_dt": "", //optional
                "is_editable": "True", // optional
                "is_private": "True" // optional
            }
        ],
        "answers": [
            1: {
                // First answer of the first question.
                1: {
                    "answer_num": "1",
                    "answer_text": "Answer 1"
                },
                2: {
                    "answer_num": "2",
                    "answer_text": "Answer 2"
                },
                ...
            },
        ]
    }
```
| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key. |
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
        "api_key": "Your api key",
        "question_title": "Your question title",
        "question_text": "Your question text",
        "start_dt": "",
        "end_dt": "",
        "is_editable": "True",
        "is_private": "True",
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
