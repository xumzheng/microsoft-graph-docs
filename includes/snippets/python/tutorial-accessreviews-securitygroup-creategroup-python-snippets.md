---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.description = 'Building security'

request_body.displayName = 'Building security'

request_body.GroupTypes([])

request_body.mailEnabled = false

request_body.mailNickname = 'buildingsecurity'

request_body.securityEnabled = true

additionalData = [
'owners@odata.bind' => ['https://graph.microsoft.com/beta/users/d3bcdff4-4f80-4418-a65e-7bf3778c5dca', ],
'members@odata.bind' => ['https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6', 'https://graph.microsoft.com/beta/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7', ],
];
request_body.additionaldata(additionalData)




request_configuration = GroupsRequestBuilderPostRequestConfiguration(
)


result = await client.groups.post(request_body = request_body)


```