---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Group()
request_body.setDescription('Group assignable to a role')

request_body.setDisplayName('Role assignable group')

request_body.setGroupTypes(['Unified', ])

request_body.setIsAssignableToRole(true)

request_body.setMailEnabled(true)

request_body.setSecurityEnabled(true)

request_body.setMailNickname('contosohelpdeskadministrators')

additionalData = [
'owners@odata.bind' => ['https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e', ],
'members@odata.bind' => ['https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0', 'https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e', ],
];
request_body.setAdditionalData(additionalData)




result = await client.groups.post(request_body)


```