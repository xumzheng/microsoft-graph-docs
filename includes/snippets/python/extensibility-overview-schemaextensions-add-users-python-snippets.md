---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = User();
request_body.setAccountEnabled(true);

request_body.setDisplayName('Adele Vance');

request_body.setMailNickname('AdeleV');

request_body.setUserPrincipalName('AdeleV@m365x72712789.onmicrosoft.com');

passwordProfile = PasswordProfile();
passwordProfile.setForceChangePasswordNextSignIn(false);

passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


request_body.setPasswordProfile($passwordProfile);
additionalData = [
'extkmpdyld2_graphLearnCourses' => request_body = Extkmpdyld2_graphLearnCourses();
		request_body.setCourseId(100);

		request_body.setCourseName('Explore Microsoft Graph');

		request_body.setCourseType('Online');


request_body.setExtkmpdyld2_graphLearnCourses($extkmpdyld2_graphLearnCourses);

];
request_body.setAdditionalData(additionalData);




result = await client.users().post(request_body);


```