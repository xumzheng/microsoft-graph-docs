---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = NoncustodialSource();
additionalData = [
'@odata.id' => 'https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.compliance().ediscovery().casesById('case-id').sourceCollectionsById('sourceCollection-id').noncustodialSourcesById('noncustodialDataSource-id').post(requestBody);


```