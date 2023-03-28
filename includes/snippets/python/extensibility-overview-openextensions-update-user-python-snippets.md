---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Extension();
$additionalData = [
'xboxGamerTag' => 'FierceAdele', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->usersById('user-id')->extensionsById('extension-id')->patch($requestBody);


```