###**update_answer**


PUT - (http://quescheetah.com/v1/questions/{questionId}/answers/{answerNum})

Update a answer_text of one answer.

**request**
```javascript
    {
        "answer_text": "New answer_text"
    }
```
| Arguments | Value | Description |
| --        | --    |
| answer_text | string | New texts to choose. |

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