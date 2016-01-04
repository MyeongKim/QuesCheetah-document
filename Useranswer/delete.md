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

**return**
```javascript
    {
        "result": "success",
        "description": "Delete description"
    }
```