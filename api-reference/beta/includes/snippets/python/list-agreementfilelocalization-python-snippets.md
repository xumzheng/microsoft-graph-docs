---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = AgreementRequestBuilder.AgreementRequestBuilderGetQueryParameters(
				expand = ["files"],
)

request_configuration = AgreementRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.termsOfUse.agreements_by_id('agreement-id').get(request_configuration = request_configuration)


```