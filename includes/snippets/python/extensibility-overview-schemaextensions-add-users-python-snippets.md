---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.account_enabled = True

request_body.displayName = 'Adele Vance'

request_body.mailNickname = 'AdeleV'

request_body.userPrincipalName = 'AdeleV@m365x72712789.onmicrosoft.com'

password_profile = PasswordProfile()
passwordProfile.force_change_password_next_sign_in = False

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.password_profile = passwordProfile
additionalData = [
'extkmpdyld2_graphLearnCourses' => request_body = Extkmpdyld2_graphLearnCourses()
		request_body.course_id = 100

		request_body.courseName = 'Explore Microsoft Graph'

		request_body.courseType = 'Online'


request_body.extkmpdyld2_graph_learn_courses = extkmpdyld2_graphLearnCourses

];
request_body.additionaldata(additionalData)





result = await client.users.post(request_body = request_body)


```