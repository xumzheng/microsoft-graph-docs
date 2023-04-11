---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EmailAuthenticationMethod()
request_body.emailAddress = 'kim@contoso.com'



request_configuration = EmailAuthenticationMethodRequestBuilderPatchRequestConfiguration(
)


result = await client.users_by_id('user-id').authentication.emailMethods_by_id('emailAuthenticationMethod-id').patch(request_body = request_body)


```