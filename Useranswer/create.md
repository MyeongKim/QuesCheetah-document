###**create_useranswer**


POST - (http://quescheetah.com/v1/questions/{questionId}/answers/{answerNum}/useranswers)

Make a new useranswer.

**request**
```javascript 
    {
        "useranswer": {
            "unique_user"   : "Unique Id"            // For the distinction between useranswers.
        }
    }
```

| Arguments | Value | Description |
| --        | --    |
| unique_user | string | unique value that will discriminate between users |


**return**
```javascript 
    {
      "useranswer": {
        "unique_user": "222",
        "created_dt": "2016-02-09T10:34:54.712",
        "answer_num": 1,
        "id": 14
      }
    }
```