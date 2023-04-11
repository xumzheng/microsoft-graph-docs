---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationContextClassReference()
request_body.id = 'c1'

request_body.displayName = 'Contoso medium'

request_body.description = 'Medium protection level defined for Contoso policy'

request_body.isAvailable = true



request_configuration = AuthenticationContextClassReferenceRequestBuilderPatchRequestConfiguration(
)


result = await client.identity.conditionalAccess.authenticationContextClassReferences_by_id('authenticationContextClassReference-id').patch(request_body = request_body)


```