---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.setDescription('IT Helpdesk to support Contoso employees')

request_body.setDisplayName('IT Helpdesk (User)')

request_body.setMailEnabled(false)

request_body.setMailNickname('userHelpdesk')

request_body.setSecurityEnabled(true)

request_body.setIsAssignableToRole(true)

additionalData = [
'owners@odata.bind' => ['https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5', ],
'members@odata.bind' => ['https://graph.microsoft.com/v1.0/users/1ed8ac56-4827-4733-8f80-86adc2e67db5', 'https://graph.microsoft.com/v1.0/users/7146daa8-1b4b-4a66-b2f7-cf593d03c8d2', ],
];
request_body.setAdditionalData(additionalData)




result = await client.groups.post(request_body, headers=)


```