###**get_useranswer_list**


GET - (http://quescheetah.com/v1/questions/{questionId}/answers/useranswers)

Get all useranswers of this answer


**return**
```javascript 
    {
      "useranswers": {
        "1": [
          {
            "id": 9,
            "created_dt": "2016-02-09T10:16:47.372",
            "unique_user": "111"
          },
          {
            "id": 10,
            "created_dt": "2016-02-09T10:17:04.901",
            "unique_user": "112"
          }
        ],
        "2": [
          {
            "id": 11,
            "created_dt": "2016-02-09T10:17:14.432",
            "unique_user": "113"
          },
          {
            "id": 12,
            "created_dt": "2016-02-09T10:17:21.946",
            "unique_user": "114"
          },
          {
            "id": 13,
            "created_dt": "2016-02-09T10:17:27.279",
            "unique_user": "115"
          }
        ],
        "3": [],
        "4": []
      }
    }
```

###**get_useranswers_of_one_answer**


GET - (http://quescheetah.com/v1/questions/{questionId}/answers/{answerNum}/useranswers)

Get a answer instance that answerNum is answer_num of this data.

**return**
```javascript 
    {
      "useranswers": {
        "1": [
          {
            "id": 9,
            "unique_user": "111",
            "created_dt": "2016-02-09T10:16:47.372"
          },
          {
            "id": 10,
            "unique_user": "112",
            "created_dt": "2016-02-09T10:17:04.901"
          }
        ]
      }
    }
```


###**get_one_useranswer**


GET - (http://quescheetah.com/v1/questions/{questionId}/answers/useranswers/{uniqueUser})

Get one useranswer data.


**return**
```javascript
    {
      "useranswers": {
        "1": {
          "created_dt": "2016-02-09T10:16:47.372",
          "unique_user": "111",
          "id": 9
        }
      }
    }
```