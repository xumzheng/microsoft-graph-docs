---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = AgreementRequestBuilderGetRequestConfiguration(
request_config = AgreementRequestBuilderGetRequestConfiguration(query_params=query_params = AgreementRequestBuilderGetQueryParameters()
query_params.expand = ["files"]

)
query_params = AgreementRequestBuilderGetQueryParameters()
query_params.expand = ["files"]

)


result = await client.identityGovernance.termsOfUse.agreements_by_id('agreement-id').get(request_config, headers=request_config)


```