---
layout: default
title: "Example - School Registration"
parent: Registration
---

# Registering a School

#### __Scenario__:  
School named __Riverdale Academy__ wants to register to our system.

#### __URL Parameters List__:
1. `school=Riverdale Academy`

#### __Complete URL__:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=register_school&school=Riverdale Academy`

#### __Returns a JSON Response:__
{% highlight json %}
    {  
    "message": "School: 'Riverdale Academy' has been added!", 
    "success": true
    }
{% endhighlight %}
Generally, the `success` key indicates whether the request has succeeded or not.  

`true` means the school registration was successful, otherwise `false` indicates that it did not.

Response code is also another indication.
