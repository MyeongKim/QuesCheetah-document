###**create_useranswer**


POST - (http://quescheetah.com/v1/questions/{questionId}/answers/{answerNum}/useranswers)

Make a new useranswer.

**request**
```javascript 
    {
        "unique_user"   : "Unique Id"            // For the distinction between useranswers.
    }
```

| Arguments | Value | Description |
| --        | --    |
| unique_user | string | unique value that will discriminate between users |


**return**
```javascript 
    {
        "useranswer": {
            "update_num": "1",
            "unique_user": "Unique Id"
        }
    }
```