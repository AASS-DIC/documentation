---
layout: post
title: "Example - Verify Student"
parent: Verification
---

#### __Scenario__:  
IT Admin of __Riverdale Academy__ school would like to verify if a student with an ID Number of __123456__ exists in their school record.

#### __URL Parameters List__: 
1. `school=Riverdale Academy`  
2. `person_type=students`
3. `id_num=123456`

#### __Complete URL__:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=verify_person&school=Riverdale Academy&person_type=students&id_num=123456`

#### __Returns a JSON Response:__
{% highlight json %}
    {
        "content": {
            "123456": {
                "f_nm": "Caroline", 
                "id_num": "123456", 
                "l_nm": "Williamson", 
                "m_nm": "Johnson", 
                "school": "Riverdale Academy"
            }
        }, 
        "message": "Student with ID Num: '123456' exists in 'Riverdale Academy'", 
        "success": true
    }
{% endhighlight %}

Invoking this API always returns the complete information of the student.