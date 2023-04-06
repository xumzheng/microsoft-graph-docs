---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Agreement()
request_body.setDisplayName('All Contoso volunteers - Terms of use')

request_body.setIsViewingBeforeAcceptanceRequired(true)


request_config = AgreementRequestBuilderPatchRequestConfiguration(
request_config = AgreementRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.identityGovernance.termsOfUse.agreements_by_id('agreement-id').patch(request_body, headers=)


```