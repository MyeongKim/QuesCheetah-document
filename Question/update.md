###**update_question**


PUT - (http://quescheetah.com/v1/questions/{questionId})

Update this question data.

Answers for this question also can be modified by this request.


**request**
```javascript
    {
        "questions": {
            "1": {
                "question_title": "Your question title 1",
                "question_text": "Your question text 1",
                "start_dt": "", //optional
                "end_dt": "", //optional
                "is_editable": false, // optional
                "is_private": false // optional
            }
        },
        "answers": {
            "1": {
                // First answer of the first question.
                "1": {
                    "answer_text": "Answer 1"
                },
                "2": {
                    "answer_text": "Answer 2"
                },
                ...
            }
        }
    }
```
| Arguments | Value | Description |
| --        | --    |
| api_key | string | The user's own api_key. |
| group_name | string | representative title of all questions.| 
| question_title | string | Title of this question. |
| question_text  | string  | Question text to ask. |
| start_dt | long | Activation time of this question. Default is current time.(YYYY-MM-DD HH:MM:ss)|
| end_dt | long | End time of this question. Default is 30 days from start date.(YYYY-MM-DD HH:MM:ss)|
| is_editable | string | Determine whether user can change the pre-answered answer.|
| is_private | string | Show question to added urls only. |
| answer_num | integer | Be criterion of descending order. Lower number will go first.|
| answer_text | string | Giving texts to choose. |


**return**
```javascript
    {
        "questions": {
            "1": {
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
                    "answer_text": "New Answer 1"
                },
                "2": {
                    "answer_text": "New Answer 2"
                }
            }
        }
    }
```