---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Extension();
additionalData = [
'xboxGamerTag' => 'FierceAdele', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.usersById('user-id').extensionsById('extension-id').patch(requestBody);


```