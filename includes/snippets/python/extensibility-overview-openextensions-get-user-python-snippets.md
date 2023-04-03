---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Extension();
additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#users(\'3fbd929d-8c56-4462-851e-0eb9a7b3a2a5\')/extensions/$entity', 
'@odata.type' => '#microsoft.graph.openTypeExtension', 
'xboxGamerTag' => 'FierceAdele', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
'id' => 'com.contoso.socialSettings', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.usersById('user-id').extensionsById('extension-id').get(requestBody);


```