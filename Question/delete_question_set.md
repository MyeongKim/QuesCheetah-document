###**delete_question_set**


POST - (http://quescheetah.com/v1/question/set/delete)

Delete one question with all related answers, useranswers.

**request**
```javascript
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id",    // Either question_title and question_id is required.
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string| The user's own api_key. |
| question_title | string | Title of this question. |
| question_id  | integer  | Id of this question. |

**return**
```javascript
    {
        "result": "success",
        "description": "Delete description"
    }
```
