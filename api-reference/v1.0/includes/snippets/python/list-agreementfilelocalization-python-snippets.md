---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AgreementRequestBuilderGetRequestConfiguration()

query_params = AgreementRequestBuilderGetQueryParameters()
query_params.expand = ["files"]

request_config.queryParameters = query_params


result = await client.identityGovernance.termsOfUse.agreementsById('agreement-id').get(request_config)


```