###**create_answer**


POST - (http://quescheetah.com/v1/questions/{questionId}/answers)

Create one or multiple answers related to the question.

**request**
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
| Arguments | Value | Description |
| --        | --    |
| answer_num | integer | Be criterion of descending order. Lower number will go first.|
| answer_text | string | Giving texts to choose. |

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