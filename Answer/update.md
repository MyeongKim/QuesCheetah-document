###**update_answer**


PUT - (http://quescheetah.com/v1/questions/{questionId}/answers)

Update answer_text property at once.

**request**
```javascript
    {
        "answers": {
            "1": {
                "answer_text": "my new answer text 1"
            },
            "2": {
                "answer_text": "my new answer text 2"
            }
        }
    }
```
| Arguments | Value | Description |
| --        | --    |
| answer_text | string | New texts to choose. |

**return**
```javascript 
    {
        "answers": {
            "1": {
                "id": 38,           // id of this answer instance
                "answer_count": 0,  // How many users voted to this answer.
                "answer_text": "my new answer text 1"
            },
            "2": {
                "id": 37,           // id of this answer instance
                "answer_count": 0,  // How many users voted to this answer.
                "answer_text": "my new answer text 2"
            }
        }
    }
```