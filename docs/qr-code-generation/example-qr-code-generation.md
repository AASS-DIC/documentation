---
layout: post
title: "Example - Generate QR Code"
parent: "QR Code Generation"
---

#### __Scenario__:  
IT Admin of __Riverdale Academy__ school would like to generate QR Code for student ID Number of __123456__.

#### __URL Parameters List__: 
1. `school=Riverdale Academy`  
2. `person_type=students`
3. `id_num=123456`

#### __Complete URL__:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=gen_qrcode&school=Riverdale Academy&person_type=students&id_num=123456`

#### __Returns an Image:__
![](/assets/images/Student_123456_Riverdale_Academy.png)

#### __Contains a JSON:__
{% highlight json %}
    {
        'f_nm': 'Caroline',
        'id_num': '123456',
        'l_nm': 'Williamson',
        'm_nm': 'Johnson',
        'school': 'Riverdale University'
    }
{% endhighlight %}

Invoking this API always returns a QR Code that contains a complete information of the student.