---
title: "Verify School"
layout: post
parent: Verification
---

#### Base Url:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=verify_school`  

#### Person Registration

To verify if a school exists in our system, append to the base url:  
`&school=<school name>&shallow=true`

*Note: Replace `<...>` with the actual value*

#### Required URL Parameter:
1. `school`  

#### Optional URL Parameter:
1. `shallow=true`
Highly Recommended  
Doesnt query the data of the given school. eg. students & teachers