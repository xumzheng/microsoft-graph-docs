---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new NoncustodialDataSource();
$requestBody.setApplyHoldToSource(false);

$dataSource = new DataSource();
$dataSource.set@odatatype('microsoft.graph.ediscovery.siteSource');

$additionalData = [
'site' => $dataSource = new Site();
$		dataSource.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


$dataSource.setSite($site);

];
$dataSource.setAdditionalData($additionalData);



$requestBody.setDataSource($dataSource);


$requestResult = $graphServiceClient.compliance().ediscovery().casesById('case-id').noncustodialDataSources().post($requestBody);


```