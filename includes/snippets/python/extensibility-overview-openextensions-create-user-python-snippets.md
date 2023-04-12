---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Extension()
request_body.@odatatype = '#microsoft.graph.openTypeExtension'

request_body.id = 'com.contoso.socialSettings'

additionalData = [
'extensionName' => 'com.contoso.socialSettings', 
'skypeId' => 'skypeId.AdeleV', 
'linkedInProfile' => 'www.linkedin.com/in/testlinkedinprofile', 
'xboxGamerTag' => 'AwesomeAdele', 
];
request_body.additionaldata(additionalData)





result = await client.users_by_id('user-id').extensions.post(request_body = request_body)


```