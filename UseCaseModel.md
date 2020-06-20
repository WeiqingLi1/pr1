# Use Case Model

*This is the template for your use case model. The parts in italics are concise explanations of what should go in the corresponding sections and should not appear in the final document.*

**Author**: \<person or team name\>
Team 23


## 1 Use Case Diagram

*This section should contain a use case diagram with all the actors and use cases for the system, suitably connected.*

Only single user in our system, which is the user.


## 2 Use Case Descriptions

*For each use case in the use case diagram, this section should contain a description, with the following elements:*

![Use Case Diagram Image](use_case_diagram.png)

---
- Requirements: When user login first time, user is allowed to enter current job details and get details saved when user click save
-  Preconditions:  
i: User has a current job
ii: No current job details stored previously
-  Postconditions: Current job details stored, then return to main menu
- Scenarios: When user first login, user is allowed to enter current job details (if user has one). After user click save, details should be stored and return to main menu. Details of current job consist of:
i. Title 
ii. Company 
iii. Location (entered as city and state) 
iv. Overall cost of living in the location (expressed as an ​index​) 
v. Yearly salary 
vi. Signing bonus 
vii. Yearly bonus 
viii. Retirement benefits (as percentage matched) 
ix. Leave time (vacation days and holiday and/or sick leave, as a single overall number of days) 
---
- Requirements: When user login first time, user is allowed to enter current job details and get details not saved if user click cancel
-  Preconditions: 
i: User has a current job
ii: No current job details stored previously
-  Postconditions: Current job details not stored, the return to main menu
- Scenarios: When user first login, user is allowed to enter current job details (if user has one). After user click cancel, details should not be stored and return to main menu. Details of current job consist of: <br/>
i. Title 
ii. Company 
iii. Location (entered as city and state) 
iv. Overall cost of living in the location (expressed as an ​index​) 
v. Yearly salary 
vi. Signing bonus 
vii. Yearly bonus 
viii. Retirement benefits (as percentage matched) 
ix. Leave time (vacation days and holiday and/or sick leave, as a single overall number of days) 
---
- Requirements: User is allowed to edits current job details and get them saved if user click save
-  Preconditions: 
i: Current job details already exist
ii: User edits current job details
-  Postconditions: Edited job details stored and override the existing current job details, then return to main menu
- Scenarios: When job details already entered previously and user wants to edit details again. When user click enter current job details, current job details displayed to user and enable user to edit any one of these details. After user click save, edited job details will be stored and override existing current job details.
---
- Requirements: User is allowed to edit current job details get them unsaved if user click cancel
-  Preconditions: 
i: Current job details already exist
ii: User edit current job details
-  Postconditions: Edited job details not stored and then return to main menu
- Scenarios: When job details already entered previously and user wants to edit details again. When user click enter current job details, current job details displayed to user and enable user to edit any one of these details. After user click cancel, edited job details will not be stored and  current job details keep the same. Then return to main menu.
---
- Requirements: User is allowed to enter job offers
-  Preconditions: User has a job offer
-  Postconditions: Job offer details stored
- Scenarios: User is allowed to enter details of job offer whenever user gets one job offer, which consist of the same ones listed for current job. 
---
- Requirements: User is allowed to compare offer with current job
-  Preconditions: 
i: User has a current job
ii: At lease one job offer stored
-  Postconditions: A table of comparing results displayed to user
- Scenarios: After one job offer entered and user has a current job whose details already stored, user is allowed to compare the offer with the current job details.
---
- Requirements: User is allowed to adjust comparison settings anytime user wants
-  Preconditions: Weights assigned to default value one or previously adjusted weights already stored
-  Postconditions: Weights stored
- Scenarios: User is allowed to adjust the comparison settings anytime user wants. User is allowed to assign integer weights to:
a. Yearly salary
b. Signing bonus
c. Yearly bonus
d. Retirement benefits
e. Leave time
---
- Requirements: ser is allowed to compare offers when and user has no current job
-  Preconditions: At lease two offers exist in list
-  Postconditions:  A table of comparing results displayed to user
- Scenarios: User is allowed to compare any two job offers chose from list of job offers. A table of comparing result shall be displayed.
---
- Requirements: When a list of ranked offers showed, user is allowed to compare offers when user has a current job
- Preconditions: 
i: At lease one offer exist in list
ii: User has a current job
iii: A list of ranked offers showed to user
-  Postconditions: A table of comparing results displayed to user
- Scenarios: User is allowed to compare any two job offers chose from list of job offers or compare current job with any job offer chosen from list. A table of comparing result shall be displayed.
---
- Requirements: User is allowed to rank job offers
-  Preconditions: At lease one offer entered
-  Postconditions: Offers in list will be ranked by weighted sum function, a list of results be displayed to user
- Scenarios: ffers in list will be ranked by weighted sum function, a list of results be displayed to user
---

<!--stackedit_data:
eyJkaXNjdXNzaW9ucyI6eyI0bEZOMnZmTHlTdFNuZHhrIjp7In
RleHQiOiJzZXIiLCJzdGFydCI6MTUxMCwiZW5kIjoxNTEwfSwi
akJISEJGelVYdGFOUlhEaiI6eyJ0ZXh0Ijoib09mZmVycyIsIn
N0YXJ0Ijo1NjkzLCJlbmQiOjU2OTN9LCJpeU9TeXRwN1dyVFhC
QWx1Ijp7InRleHQiOiJmZmVycyIsInN0YXJ0Ijo1ODQ0LCJlbm
QiOjU4NDR9fSwiY29tbWVudHMiOnsiZkZqTW9walNZMFh4RGxI
cSI6eyJkaXNjdXNzaW9uSWQiOiI0bEZOMnZmTHlTdFNuZHhrIi
wic3ViIjoiZ286MTEzMTA1OTEzMzk4NzE0OTQ0NDE5IiwidGV4
dCI6InNwZWxsaW5nIiwiY3JlYXRlZCI6MTU5MjYxNTQ5NjY3MH
0sIjBma0dZejNOVGIwaWx2RHYiOnsiZGlzY3Vzc2lvbklkIjoi
akJISEJGelVYdGFOUlhEaiIsInN1YiI6ImdvOjExMzEwNTkxMz
M5ODcxNDk0NDQxOSIsInRleHQiOiJ0eXBvIiwiY3JlYXRlZCI6
MTU5MjYxNTU4ODczOX0sIkhCbjZYRXVINmszZ2FSVUYiOnsiZG
lzY3Vzc2lvbklkIjoiaXlPU3l0cDdXclRYQkFsdSIsInN1YiI6
ImdvOjExMzEwNTkxMzM5ODcxNDk0NDQxOSIsInRleHQiOiJ0eX
BvIiwiY3JlYXRlZCI6MTU5MjYxNTYwNDgxNH19LCJoaXN0b3J5
IjpbMTIwMTU0OTk4MCwxMzgzODMzNzE5LDEwMzc0MTgzODAsMT
YzMTY1MzE2Nyw4ODczNjQwNjcsMjA2MTE3OTAyLC0yMDc0Nzky
OTczLDYwNTYwMjk4NCwtOTc2MDE1NzAwLC0xNzMyMzM5ODY3LC
01NDc2NzgwNTEsLTEzMDEyNjE4ODEsLTgyNDE0ODY4MCwzNzUz
NDYxMTAsLTMzNDk5MjYyNiwxMTIzODU5MTI3LDM2Mzk3ODcyMi
wtMTk1NTMxMjUzMywxODUzMzUxMjEsLTE2NTg2NzIxMTFdfQ==

-->
