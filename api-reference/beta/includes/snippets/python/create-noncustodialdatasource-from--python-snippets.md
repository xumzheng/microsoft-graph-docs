---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialSource()
additionalData = [
'@odata.id' => 'https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246', 
];
request_body.setAdditionalData(additionalData)



request_config = NoncustodialDataSourceRequestBuilderPostRequestConfiguration(
request_config = NoncustodialDataSourceRequestBuilderPostRequestConfiguration(query_params=)


await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').noncustodialSources_by_id('noncustodialDataSource-id').post(request_body, headers=)


```