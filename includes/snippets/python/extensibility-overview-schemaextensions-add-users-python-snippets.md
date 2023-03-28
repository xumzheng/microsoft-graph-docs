---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new User();
$requestBody.setAccountEnabled(true);

$requestBody.setDisplayName('Adele Vance');

$requestBody.setMailNickname('AdeleV');

$requestBody.setUserPrincipalName('AdeleV@m365x72712789.onmicrosoft.com');

$passwordProfile = new PasswordProfile();
$passwordProfile.setForceChangePasswordNextSignIn(false);

$passwordProfile.setPassword('xWwvJ]6NMw+bWH-d');


$requestBody.setPasswordProfile($passwordProfile);
$additionalData = [
'extkmpdyld2_graphLearnCourses' => $requestBody = new Extkmpdyld2_graphLearnCourses();
		$requestBody.setCourseId(100);

$		requestBody.setCourseName('Explore Microsoft Graph');

$		requestBody.setCourseType('Online');


$requestBody.setExtkmpdyld2_graphLearnCourses($extkmpdyld2_graphLearnCourses);

];
$requestBody.setAdditionalData($additionalData);




$requestResult = $graphServiceClient.users().post($requestBody);


```