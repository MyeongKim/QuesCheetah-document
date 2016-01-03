###**to_private**


POST - (http://quescheetah.com/v1/question/private)

Change question state to private.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id"    // Either question_title and question_id is required.
    }

```

**return**
``` 
    {}
```
    
###**to_public**


POST - (http://quescheetah.com/v1/question/public)

Change question state to public.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id"    // Either question_title and question_id is required.
    }

```

**return**
``` 
    {}
```
    
###**get_url_list**


POST - (http://quescheetah.com/v1/question/url/list)

Get authenticated urls of the question.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id"    // Either question_title and question_id is required.
    }

```

**return**
``` 
    {
        'urls': {0:{"https://naver.com"},
                 1:{"https://google.com"},
                 2:{"https://daum.net"},
                 ...
                 }
    }
```
    
###**add_url**


POST - (http://quescheetah.com/v1/question/url/add)

Add an authenticated url.

**request**
``` 
    {
        'api_key'       : "Your api key",
        'question_title': "Your question title",
        'question_id'   : "Your question id",    // Either question_title and question_id is required.
        'url'           : "New url"
    }

```

**return**
``` 
    {
        'urls': {0:{"https://naver.com"},
                 1:{"https://google.com"},
                 2:{"https://daum.net"},
                 ...
                 }
    }
```