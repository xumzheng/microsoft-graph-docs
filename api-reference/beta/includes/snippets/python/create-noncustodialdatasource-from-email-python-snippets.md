---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = NoncustodialDataSource();
requestBody.setApplyHoldToSource(true);

dataSource = DataSource();
dataSource.set@odatatype('microsoft.graph.ediscovery.userSource');

additionalData = [
'email' => 'adelev@contoso.com', 
];
dataSource.setAdditionalData(additionalData);



requestBody.setDataSource($dataSource);


requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').noncustodialDataSources().post(requestBody);


```