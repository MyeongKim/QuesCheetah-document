###**delete_multi_question_set**


POST - (http://quescheetah.com/v1/multiple/delete)

Delete one group with all related questions, answers, useranswers.

**request**
```javascript
    {
        "api_key"       : "Your api key",
        "group_name"    : "Your group name"
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string | The user's own api_key. |
| group_name | string | representative title of all questions.| 


**return**
```javascript
    {
        "result": "success",
        "description": "Delete description"
    }
```
