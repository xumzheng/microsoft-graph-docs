---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
request_body.description = 'Feelgood Marketing Campaign with external partners and vendors.'

request_body.displayName = 'Feelgood Marketing Campaign'

request_body.GroupTypes(['Unified', ])

request_body.mailEnabled = true

request_body.mailNickname = 'FeelGoodCampaign'

request_body.securityEnabled = true

additionalData = [
'owners@odata.bind' => ['https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7', ],
'members@odata.bind' => ['https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20', ],
];
request_body.additionaldata(additionalData)




request_configuration = GroupsRequestBuilderPostRequestConfiguration(
)


result = await client.groups.post(request_body = request_body)


```