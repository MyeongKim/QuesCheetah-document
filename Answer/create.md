###**create_answer**


POST - (http://quescheetah.com/v1/questions/{questionId}/answers)

Create one or multiple answers related to the question.

**request**
```javascript
    {
        "answers": {
            "1": {
                "answer_text": "my answer text 1"
            },
            "2": {
                "answer_text": "my answer text 2"
            }
        }
    }
```
| Arguments | Value | Description |
| --        | --    |
| answer_text | string | Giving texts to choose. |

**return**
```javascript 
    {
        "answers": {
            "1": {
                "id": 38,           // id of this answer instance
                "answer_count": 0,  // How many users voted to this answer.
                "answer_text": "my answer text 1"
            },
            "2": {
                "id": 37,           // id of this answer instance
                "answer_count": 0,  // How many users voted to this answer.
                "answer_text": "my answer text 2"
            }
        }
    }
```