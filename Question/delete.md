###**delete_question**


DELETE - (http://quescheetah.com/v1/questions/{questionId})

Delete one question. All related answers and useranswers are deleted together.

**return**
```javascript
    {
        "result": "success",
        "description": "Deleted a question."
    }
```