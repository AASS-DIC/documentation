---
layout: post
title: "Example - Student Registration"
parent: Registration
---

#### __Scenario__:  
__Riverdale Academy__ wants to register a student called __Caroline Johnson Williamson__ with an ID Num of __123456__ to our system.

#### __URL Parameters List__:
1. `school=Riverdale Academy`
2. `f_nm=Caroline`
3. `m_nm=Johnson`
4. `l_nm=Williamson`
5. `id_num=123456`

#### __Complete URL__:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=register_person&school=Riverdale Academy&person_type=students&f_nm=Caroline&m_nm=Johnson&l_nm=Williamson&id_num=123456`

#### __Returns a JSON Response:__
{% highlight json %}
    {
    "message": "Student '123456' 'Caroline Johnson Williamson' was added to 'Riverdale Academy'", 
    "received data": {
        "f_nm": "Caroline", 
        "id_num": "123456", 
        "l_nm": "Williamson", 
        "m_nm": "Johnson", 
        "school": "Riverdale Academy"
    }, 
    "success": true
    }
{% endhighlight %}