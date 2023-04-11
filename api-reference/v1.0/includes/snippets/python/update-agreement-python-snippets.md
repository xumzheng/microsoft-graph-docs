---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Agreement()
request_body.displayName = 'All Contoso volunteers - Terms of use'

request_body.isViewingBeforeAcceptanceRequired = true



request_configuration = AgreementRequestBuilderPatchRequestConfiguration(
)


result = await client.identityGovernance.termsOfUse.agreements_by_id('agreement-id').patch(request_body = request_body)


```