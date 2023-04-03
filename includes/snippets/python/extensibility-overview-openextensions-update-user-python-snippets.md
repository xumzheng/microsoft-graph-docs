---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Extension();
additionalData = [
'xboxGamerTag' => 'FierceAdele', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
];
requestBody.setAdditionalData(additionalData);




result = await client.usersById('user-id').extensionsById('extension-id').patch(requestBody);


```