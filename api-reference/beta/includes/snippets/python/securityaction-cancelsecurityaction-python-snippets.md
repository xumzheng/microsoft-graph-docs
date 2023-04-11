---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = CancelSecurityActionRequestBuilderPostRequestConfiguration(
)


await client.security.securityActions_by_id('securityAction-id').cancelSecurityAction.post()


```