# SignUp api: POST:

**http://localhost:8000/auth/SignUp**


```
{
  "email": "testuser@example.com",
  "password": "securepassword",
  "name": "Test User",
  "age": 25,
  "weight": 70.5
}

```

---

# Login api: POST:

**http://localhost:8000/auth/Login**


```
{
  "email": "testuser@example.com",
  "password": "securepassword"
}
```


---




# Get User Info : GET

**http://localhost:5004/auth/User**



"Authorization" : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"



---






# Add Assesment result : POST

**http://localhost:5004/addassesment/assessments**

**Header**

"Authorization":  "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTc0OTE1NDY4MiwiZXhwIjoxNzQ5NzU5NDgyfQ.veKJMkAwIJcnafv2XOV9ZTu1zlQBJTHxc4-gzcbq6rk"

```
{
  "assessmentName": "Anxiety Level Test",
  "assessmentResult": "Severe anxiety",
  "assessmentScore": "40 out of 40",
  "recommendation": "Your anxiety levels are high. It's recommended to seek professional help for proper evaluation and support.",
  "takenAt": "2025-06-05T19:01:03.946Z"
}
```


---


# Delete Assessment : DELETE

**http://localhost:5004/addassesment/assessments/109**


**Header**

"Authorization":  "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjEsImlhdCI6MTc0OTE1NDY4MiwiZXhwIjoxNzQ5NzU5NDgyfQ.veKJMkAwIJcnafv2XOV9ZTu1zlQBJTHxc4-gzcbq6rk"


---




# Get assesment by User : GET

**http://localhost:5004/addassesment/getassessments**

**Header**

Authorization : Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A




---




# Add Mood  : Post

**http://localhost:5004/mood/addmood/**


**Header**
"Authorization" : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"



```
{
"mood": "Happy",
"notes": "Had a great day at work and spent time with friends.",
"time": "2025-06-06T18:30:00Z"
}
```

---


# Delete Mood :DELETE

**http://localhost:5004/mood/delmood/2**

**Header**
"Authorization" : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"



---


# GEt mood my User :GET

**http://localhost:5004/mood/getMood/**

**Header**
"Authorization" : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"


---






# Add activity : Post 

**http://localhost:5004/activity/addactivity/**

**Header**

Authorization : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"



```
{
  "activity": "Happy",
  "notes": "Had a great day at work",
  "time": "2025-06-07T18:30:00"
}

```


---


# Delete Activity : delete

**http://localhost:5004/activity/delactivity/2**


**Header**

"Autheraztion" : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"


---



# Get Activity By User 


**http://localhost:5004/activity/getActivity/**


**Header**

Authorization : "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VySWQiOjMsImlhdCI6MTc0OTIyNTE1OCwiZXhwIjoxNzQ5ODI5OTU4fQ.ynbnzUJrPyEnNLh_EVdNA8kJlPbK-ufC4oBRSbKRo6A"




---



 







---
----
---
---
---

# GAME


# save game score and get game assesment : POST

**http://localhost:5004/game/gameScore/**

**Header**
send autherization token


```
{
  "game_name": "flappy bird",
  "game1Score": 111,
  "game2Score": 11,
  "game3Score": 12
}
```

---

# GET game Rank : GET

**http://localhost:5004/game//gameRank/flappy bird**

**Header**
AUtheraztion : token


---



# Post Game assessment : POST

**http://localhost:5004/game/gameassessment**

**Header**

Autherization : Token



```
{
  "game_name": "flappy bird",
  "recommendation": "You have shown improvement. Focus on enhancing your reaction time and managing stress for better scores.",
  "attention": 78,
  "focus": 75,
  "short_term_memory": 72,
  "reaction_time": 68,
  "working_memory": 74,
  "hand_eye_coordination": 70,
  "stress_response": 65,
  "feedback": "Great progress this week!"
}
```

---

# Get User Game assessment Data : GET

**http://localhost:5004/game/gameassessmentData**

**Header**

Autheraztion : Token


---
---
---
---



# Save Doctor : POST 

**http://localhost:5004/doctor/addDoctor/**

**Header**
Autherization : Token


```
{
"name": "Prof. Dr. Md. Rezaul Karim",
"title": "MBBS, FCPS (Psychiatry), MS (USA)",
"position": "Psychiatry (Brain, Mental Diseases, Drug Addiction) Specialist",
"teaches": "Former Professor & Head, Psychiatry, Sylhet MAG Osmani Medical College & Hospital",
"city": "Sylhet",
"chamber": "Zindabazar Point, Sylhet",
"phone": "+8801712345678"
}
```



---


# GET all doctor : GET 

**http://localhost:5004/doctor/getallDoctor**



---


# Recommand a Doctor : POST 

**http://localhost:5004/doctor/recommandDoctor**

**Header**

"Autherization": Token,


```
{
  "assessmentData": true,
  "moodData": true,
  "activityData": false,
  "city": "Sylhet"
}
```


---



# Counselor Context API : POST

**http://localhost:5004/counselor/context**

**Header**
Authrization : Token


```
{
  "selectedAssessmentsId": [
    "6849d1c07e13a8dc0e2ea81a",
    "6849d17d7e13a8dc0e2ea816",
    "68472c9d275a2b1cfa48b66c",
    "68472c4f275a2b1cfa48b662",
    "68472c30275a2b1cfa48b660",
    "68472c02275a2b1cfa48b65e"
  ],
  "moodHistory": 5,
  "activityHistory": 5,
  "gameHistory": 7
}
```

---




# research

**http://localhost:5004/research/research**

```

{
  "email": "user@example.com",
  "Q1": 3,
  "Q2": 4,
  "Q3": 2,
  "Q4": 5,
  "Q5": 1,
  "Q6": 4,
  "Q7": 3,
  "Q8": 2,
  "Q9": 5,
  "Q10": 1,
  "Q11": 4,
  "Q12": 3,
  "Q13": 2,
  "Q14": 5,
  "Q15": 1,
  "Q16": 4,
  "Q17": 3,
  "Q18": 2,
  "Q19": 5,
  "Q20": 1,
  "Q21": 4,
  "Q22": 3,
  "Q23": 2,
  "Q24": 5,
  "Q25": 1,
  "Q26": 4,
  "Q27": 3,
  "Q28": 2,
  "Q29": 5,
  "Q30": 1,
  "Q31": 4,
  "Q32": 3,
  "Q33": 2,
  "Q34": 5,
  "Q35": 1,
  "Q36": 4,
  "Q37": 3,
  "Q38": 2,
  "Q39": 5,
  "Q40": 1,
  "Q41": 4,
  "Q42": 3,
  "Q43": 2,
  "Q44": 5,
  "Q45": 1,
  "Q46": 4,
  "Q47": 3,
  "Q48": 2,
  "Q49": 5,
  "Q50": 1,
  "Q51": 4,
  "Q52": 3,
  "Q53": 2,
  "Q54": 5,
  "Q55": 1
}
```