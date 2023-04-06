---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CustodianSource()
additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531', 
];
request_body.setAdditionalData(additionalData)



request_config = DataSourceRequestBuilderPostRequestConfiguration(
request_config = DataSourceRequestBuilderPostRequestConfiguration(query_params=)


await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').custodianSources_by_id('dataSource-id').post(request_body, headers=)


```