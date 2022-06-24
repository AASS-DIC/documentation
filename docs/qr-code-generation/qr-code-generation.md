---
title: "QR Code Generation"
layout: default
has_children: true
---

#### Base Url:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=gen_qrcode`  

#### Generate QR Code

To generate a QR Code for a person in a school, append to the base url:  
`&school=<school name>&person_type=<type of person>&id_num=<id number>&image_format=<image format>`

*Note: Replace `<...>` with the actual value*

#### Required URL Parameter:
1. `school`  

2. `person_type`  

3. `id_num`  

#### Optional URL Parameter:
1. `image_format`  
Default Value: `png`  
Alt Value: `svg`    -   gives SVG as the output image type