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
| api_key | string| The user's own api_key. |
| question_title | string | Title of this question. |
| question_text  | string  | Question text to ask. |
| start_dt | long | Activation time of this question. Default is current time.|
| end_dt | long | End time of this question. Default is 30 days from start date.|
| is_editable | string | Determine whether user can change the pre-answered answer.|
| is_private | string | Show question to added urls only. |
| answer_num | integer | Be criterion of descending order. Lower number will go first.|
| answer_text | string | Giving texts to choose. |


**return**
```javascript
    {
        "result": "success",
        "description": "Delete description"
    }
```
