---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SourceCollection();
requestBody.setDisplayName('Quarterly Financials search');



result = awaitclient.compliance().ediscovery().casesById('case-id').sourceCollectionsById('sourceCollection-id').patch(requestBody);


```