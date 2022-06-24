---
title: "Student Registration"
layout: default
parent: Registration
---

#### Base Url:  
`https://aass-dic-backend.lonewanderer27.repl.co/api/?request_type=register_person`  

#### Student Registration

To register a student under a school, append the following to the base url:  
`&school=<school name>&person_type=students&id_num=<id number>&f_nm=<first name>&m_mn=<middle name>&l_nm=<last name>&section=<section>&gender=<gender>&course=<course>&gr_lvl=<grade level>&yr_lvl=<year level>&date_of_birth=<date of birth>`

*Replace the `< ... >` with the actual value*

#### Required URL Parameters:
1. `id_num`  
For students it's commonly called Learner Reference Number or LRN.  It can consist of a combination of letters, numbers and safe symbols, but not spaces:  
✅ `19-01336`  
✅ `501141600721`  
🚫 `3wts6 5gsw`

2. `f_nm`  

3. `l_nm`  

4. `person_type`  

5. `school`  


#### Optional URL Parameters:
1. `m_nm`  

2. `section`

3. `gender`

4. `course`

5. `gr_lvl`

6. `yr_lvl`

7. `date_of_birth`  
Format:     `YYYY-MM-DD`  
Example:    `2003-05-27`
