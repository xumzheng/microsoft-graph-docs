---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EmailAuthenticationMethod()
request_body.setEmailAddress('kim@contoso.com')



result = await client.usersby_id('user-id')_authentication_emailMethodsby_id('emailAuthenticationMethod-id').patch(request_body)


```