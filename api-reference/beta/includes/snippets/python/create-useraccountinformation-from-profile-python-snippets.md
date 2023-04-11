---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UserAccountInformation()
request_body.AllowedAudiences(AllowedAudiences('organization'))

request_body.countryCode = 'NO'



request_configuration = AccountRequestBuilderPostRequestConfiguration(
)


result = await client.me.profile.account.post(request_body = request_body)


```