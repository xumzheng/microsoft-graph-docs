---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
additionalData = [
'@odata.context' => 'https://graph.microsoft.com/beta/$metadata#users(\'3fbd929d-8c56-4462-851e-0eb9a7b3a2a5\')/extensions/$entity', 
'@odata.type' => '#microsoft.graph.openTypeExtension', 
'xboxGamerTag' => 'FierceAdele', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
'id' => 'com.contoso.socialSettings', 
];
request_body.setAdditionalData(additionalData)




result = await client.users_by_id('user-id').extensions_by_id('extension-id').get(request_body)


```