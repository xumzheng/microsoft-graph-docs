---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CustodianSource();
$additionalData = [
'@odata.id' => 'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/ab3a628a383045eba344b3caecba3104/userSources/31423539-3846-4333-4136-353644383531', 
];
$requestBody.setAdditionalData($additionalData);




$graphServiceClient.compliance().ediscovery().casesById('case-id').sourceCollectionsById('sourceCollection-id').custodianSourcesById('dataSource-id').post($requestBody);


```