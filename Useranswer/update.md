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
        "answer_num": 3,
        "created_dt": "2016-02-09T10:34:54.712",
        "id": 14,
        "unique_user": "222"
      }
    }
```