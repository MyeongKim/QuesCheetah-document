###**get_useranswers_of_group**


GET - (http://quescheetah.com/v1/groups/{groupId}/answers/useranswers)

Get all useranswers of this group


**return**
```javascript 
    {
      "useranswers": {
        "1": {
          "1": [
            {
              "id": 1,
              "created_dt": "2016-03-04T08:08:14.706",
              "unique_user": "1457078894675"
            },
            {
              "id": 4,
              "created_dt": "2016-03-04T08:09:14.944",
              "unique_user": "1457078954915"
            },
            {
              "id": 7,
              "created_dt": "2016-03-04T08:11:55.470",
              "unique_user": "1457079115450"
            }
            }
          ],
          "2": [
          {
              "id": 23,
              "created_dt": "2016-03-04T08:15:40.913",
              "unique_user": "1457079340895"
            },
            {
              "id": 26,
              "created_dt": "2016-03-04T08:16:05.332",
              "unique_user": "1457079365312"
            },
            {
              "id": 29,
              "created_dt": "2016-03-04T08:21:04.800",
              "unique_user": "1457079664781"
            }]
        },
        "2": {
          "1": [
            {
              "id": 2,
              "created_dt": "2016-03-04T08:08:21.184",
              "unique_user": "1457078901147"
            }
          ],
          "2": [
            {
              "id": 30,
              "created_dt": "2016-03-04T08:21:05.760",
              "unique_user": "1457079665734"
            }
          ]
        },
        "3": {
          "1": [
            {
              "id": 6,
              "created_dt": "2016-03-04T08:09:17.825",
              "unique_user": "1457078957794"
            },
            {
              "id": 9,
              "created_dt": "2016-03-04T08:11:56.686",
              "unique_user": "1457079116668"
            }
          ]
        }
      }
    }
```


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