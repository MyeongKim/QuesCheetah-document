###**create_useranswer**


POST - (http://quescheetah.com/v1/useranswer/create)

Make a new useranswer.

**request**
```javascript 
    {
        "api_key"       : "Your api key",
        "question_title": "Your question title",
        "question_id"   : "Your question id",    // Either question_title and question_id is required.
        "update_num"    : "1",                    // The answer_num of answer
        "unique_user"   : "Unique Id"            // For the distiction between useranswers.
    }
```

| Arguments | Value | Description |
| --        | --    |
| api_key | string | The user's own api_key. |
| question_title | string | Title of this question. |
| question_id  | integer  | Id of this question. |
| update_num | integer | answer_num value of selected answer |
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