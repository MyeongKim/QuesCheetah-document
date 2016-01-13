###**delete_useranswer**


POST - (http://quescheetah.com/v1/useranswer/delete)

Delete one useranswer.

**request**
```javascript
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id",    // Either question_title and question_id is required.
        "answer_num"    : "Your answer number",
        "unique_user"   : "Unique Id"
    }
```
| Arguments | Value | Description |
| --        | --    |
| api_key | string | The user's own api_key. |
| question_title | string | Title of this question. |
| question_id  | integer  | Id of this question. |
| answer_num | integer | Be criterion of descending order. Lower number will go first.|
| unique_user | string | unique value that will discriminate between users |


**return**
```javascript
    {
        "result": "success",
        "description": "Delete description"
    }
```