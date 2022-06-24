---
layout: post
title: "Example - Verify School"
parent: Verification
---

#### __Scenario__:  
An IT Admin would like to verify if __Riverdale Academy__ already exists in our system

#### __URL Parameters List__: 
1. `school=Riverdale Academy`  

#### __Complete URL__:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=verify_school&school=Riverdale Academy`

#### __Returns a JSON Response:__
{% highlight json %}
    {
    "content": {
        "Riverdale Academy": {
        "students": {
            "123456": {
                "f_nm": "Caroline", 
                "id_num": "123456", 
                "l_nm": "Williamson", 
                "m_nm": "Johnson", 
                "school": "Riverdale Academy"
            }
        }
    }, 
    "message": "School: 'Riverdale Academy' has been found!", 
    "success": true
    }
{% endhighlight %}

Invoking this API always returns the people in the given school, namely students and teachers.

Following the previous examples, remember that we have registered __Riverdale Academy__, and we have also registered __Caroline__ in that school so the API Response shows it in here in `content` key.

# Shallow Query

To avoid slow response, it is recommended to only do shallow querying which doesn't include the data inside the school, eg. students and teachers.  

Add this line to Complete URL above:  

`&shallow=true`

#### __Returns a JSON Response:__
{% highlight json %}
    {
    "content": "Riverdale Academy", 
    "message": "School: 'Riverdale Academy' has been found!", 
    "success": true
    }
{% endhighlight %}