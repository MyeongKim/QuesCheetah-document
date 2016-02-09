###**get_answer_list**


GET - (http://quescheetah.com/v1/questions/{questionId}/answers)

Get all answer data related with one question.


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

###**get_one_answer**


GET - (http://quescheetah.com/v1/questions/{questionId}/answers/{answerNum})

Get a answer instance that answerNum is answer_num of this data.

**return**
```javascript 
    {
        "answers": {
            "1": {
                "id": 38,           // id of this answer instance
                "answer_count": 0,  // How many users voted to this answer.
                "answer_text": "my answer text 1"
            }
        }
    }
```