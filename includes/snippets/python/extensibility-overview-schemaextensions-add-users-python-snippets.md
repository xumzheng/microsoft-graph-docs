---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = User()
request_body.accountEnabled = true

request_body.displayName = 'Adele Vance'

request_body.mailNickname = 'AdeleV'

request_body.userPrincipalName = 'AdeleV@m365x72712789.onmicrosoft.com'

passwordProfile = PasswordProfile()
passwordProfile.forceChangePasswordNextSignIn = false

passwordProfile.password = 'xWwvJ]6NMw+bWH-d'


request_body.passwordProfile = passwordProfile
additionalData = [
'extkmpdyld2_graphLearnCourses' => request_body = Extkmpdyld2_graphLearnCourses()
		request_body.courseId = 100

		request_body.courseName = 'Explore Microsoft Graph'

		request_body.courseType = 'Online'


request_body.extkmpdyld2_graphLearnCourses = extkmpdyld2_graphLearnCourses

];
request_body.additionaldata(additionalData)





result = await client.users.post(request_body = request_body)


```