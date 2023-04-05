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




await client.compliance.ediscovery.cases._by_id('case-id').sourceCollections._by_id('sourceCollection-id').noncustodialSources._by_id('noncustodialDataSource-id').post(request_body)


```