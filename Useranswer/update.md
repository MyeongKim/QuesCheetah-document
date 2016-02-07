###**update_useranswer**


PUT - (http://quescheetah.com/v1/questions/{questionId}/answers/{answerNum}/useranswers/{uniqueUser})

Update the answer_num of useranswer instance.

**request**
```javascript 
    {
        "answer_num"   : "Number to change"
    }
```

| Arguments | Value | Description |
| --        | --    |
| answer_num | integer | New answer_num value for useranswer|


**return**
```javascript 
    {
        "useranswer": {
            "answer_num": "1",
            "unique_user": "Unique Id"
        }
    }
```