###**delete_answer**


POST - (http://quescheetah.com/v1/answer/delete)

Delete one answer. Not including related data.

**request**
```
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id",    // Either question_title and question_id is required.
        'answer_num'    : "Your answer number"
    }

```

**return**
```
    {}
```