---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Extension();
requestBody.set@odatatype('#microsoft.graph.openTypeExtension');

requestBody.setId('com.contoso.socialSettings');

additionalData = [
'extensionName' => 'com.contoso.socialSettings', 
'skypeId' => 'skypeId.AdeleV', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
'xboxGamerTag' => 'AwesomeAdele', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.usersById('user-id').extensions().post(requestBody);


```