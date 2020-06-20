# Use Case Model

*This is the template for your use case model. The parts in italics are concise explanations of what should go in the corresponding sections and should not appear in the final document.*

**Author**: Team 23


## 1 Use Case Diagram

*This section should contain a use case diagram with all the actors and use cases for the system, suitably connected.*

Only single user in our system, which is the user.
![Use Case Diagram Image](use_case_diagram.png)

## 2 Use Case Descriptions

*For each use case in the use case diagram, this section should contain a description, with the following elements:*


---
#### Use Case 1
- Requirements: When user login first time, user is allowed to enter current job details and get details saved when user click save
-  Preconditions: <br/>
i: User has a current job <br/>
ii: No current job details stored previously <br/>
-  Postconditions: Current job details stored, then return to main menu
- Scenarios: When user first login, user is allowed to enter current job details (if user has one). After user click save, details should be stored and return to main menu. Details of current job consist of:  
i. Title   <br/>
ii. Company   <br/>
iii. Location (entered as city and state) <br/>
iv. Overall cost of living in the location (expressed as an ​index​) <br/>
v. Yearly salary <br/>
vi. Signing bonus <br/>
vii. Yearly bonus <br/>
viii. Retirement benefits (as percentage matched) <br/>
ix. Leave time (vacation days and holiday and/or sick leave, as a single overall number of days) <br/>
---
#### Use Case 2
- Requirements: When user login first time, user is allowed to enter current job details and get details not saved if user click cancel
-  Preconditions:  <br/>
i: User has a current job<br/>
ii: No current job details stored previously<br/>
-  Postconditions: Current job details not stored, then return to main menu
- Scenarios: When user first login, user is allowed to enter current job details (if user has one). After user click cancel, details should not be stored and return to main menu. Details of current job consist of: <br/>
i. Title <br/>
ii. Company <br/>
iii. Location (entered as city and state) <br/>
iv. Overall cost of living in the location (expressed as an ​index​) <br/>
v. Yearly salary <br/>
vi. Signing bonus <br/>
vii. Yearly bonus <br/>
viii. Retirement benefits (as percentage matched) <br/>
ix. Leave time (vacation days and holiday and/or sick leave, as a single overall number of days) <br/>
---
#### Use Case 3
- Requirements: User is allowed to edit current job details and get them saved if user click save
-  Preconditions:  <br/>
i: Current job details already exist<br/>
ii: User edits current job details<br/>
-  Postconditions: Edited job details stored and override the existing current job details, then return to main menu
- Scenarios: When job details already entered previously and user wants to edit details again, user can click enter current job details, then current job details displayed to user and it's allowed for user to edit any one of these details. After user click save, edited job details will be stored and override existing current job details.
---
#### Use Case 4
- Requirements: User is allowed to edit current job details get them unsaved if user click cancel
-  Preconditions:  <br/>
i: Current job details already exist<br/>
ii: User edit current job details<br/>
-  Postconditions: Edited job details not stored and then return to main menu
- Scenarios: When job details already entered previously and user wants to edit details again, user can click enter current job details, then current job details displayed to user and it's allowed for user to edit any one of these details. After user click cancel, edited job details will not be stored and current job details keep the same. Then return to main menu.
---
#### Use Case 5
- Requirements: User is allowed to enter job offers
-  Preconditions: User has a job offer
-  Postconditions: Job offer details stored
- Scenarios: User is allowed to enter details of a job offer whenever user gets one job offer, which consist of the same ones listed for current job. 
---
#### Use Case 6
- Requirements: User is allowed to compare offer with current job
-  Preconditions:  <br/>
i: User has a current job<br/>
ii: At lease one job offer stored<br/>
-  Postconditions: A table of comparing results displayed to user
- Scenarios: After one job offer entered and user has a current job whose details already stored, user is allowed to compare this offer with the current job details.
---
#### Use Case 7
- Requirements: User is allowed to adjust comparison settings anytime user wants
-  Preconditions: Weights assigned to default value - 1 or previously adjusted weights already stored
-  Postconditions: Weights stored
- Scenarios: User is allowed to adjust the comparison settings anytime user wants. User is allowed to assign integer weights to: <br/>
a. Yearly salary<br/>
b. Signing bonus<br/>
c. Yearly bonus<br/>
d. Retirement benefits<br/>
e. Leave time<br/>
---
#### Use Case 8
- Requirements: When a list of ranked offers showed, user is allowed to compare offers when user has no current job
-  Preconditions: <br/>
i: A list of ranked offers showed to user<br/>
ii: User has no current job<br/>
iii: At lease two offers exist in list<br/>
-  Postconditions:  A table of comparing results displayed to user
- Scenarios: User is allowed to compare any two job offers chosen from list of job offers if user has no current job. A table of comparing result shall be displayed.
---
#### Use Case 9
- Requirements: When a list of ranked offers showed, user is allowed to compare offers when user has a current job
- Preconditions:  <br/>
i: A list of ranked offers showed to user<br/>
ii: User has a current job<br/>
iii: At lease one offer exist in list<br/>
-  Postconditions: A table of comparing results displayed to user
- Scenarios: User is allowed to compare any two offers chosen from list of job offers or compare current job with any job offer chosen from list. A table of comparing result shall be displayed.
---
#### Use Case 10
- Requirements: User is allowed to rank job offers
-  Preconditions: At lease one offer entered
-  Postconditions: Offers in list will be ranked by weighted sum function, a list of results be displayed to user
- Scenarios: When user click compare job offers, offers in list will be ranked by weighted sum function which defined inside rank function, a list of results shall be displayed to user
---
