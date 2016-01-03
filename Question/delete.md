###**delete_question**


POST - (http://quescheetah.com/v1/question/delete)

Delete one question. Not including related data.

**request**
```
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id",    // Either question_title and question_id is required.
    }

```

**return**
```
    {}
```