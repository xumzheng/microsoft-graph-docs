---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = NoncustodialDataSource();
requestBody.setApplyHoldToSource(false);

dataSource = DataSource();
dataSource.set@odatatype('microsoft.graph.ediscovery.siteSource');

additionalData = [
'site' => dataSource = Site();
		dataSource.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


dataSource.setSite($site);

];
dataSource.setAdditionalData(additionalData);



requestBody.setDataSource($dataSource);


requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').noncustodialDataSources().post(requestBody);


```