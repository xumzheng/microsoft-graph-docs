---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryNoncustodialDataSource();
dataSource = DataSource();
dataSource.set@odatatype('microsoft.graph.security.siteSource');

additionalData = [
'site' => dataSource = Site();
		dataSource.setWebUrl('https://m365x809305.sharepoint.com/sites/Design-topsecret');


dataSource.setSite($site);

];
dataSource.setAdditionalData(additionalData);



requestBody.setDataSource($dataSource);


result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').noncustodialDataSources().post(requestBody);


```