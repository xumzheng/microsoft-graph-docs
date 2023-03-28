---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new IndustryDataConnector();
$requestBody->set@odatatype('#microsoft.graph.industryData.azureDataLakeConnector');

$requestBody->setDisplayName('CSV connector');

$additionalData = [
'sourceSystem@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/sourceSystems(\'aa050107-5784-4a8e-1876-08daddab21bc\')', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->external()->industryData()->dataConnectors()->post($requestBody);


```