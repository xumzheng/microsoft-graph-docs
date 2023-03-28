---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new PrinterShare();
$requestBody->setDisplayName('ShareName');

$requestBody->setAllowAllUsers(true);

$additionalData = [
'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->print()->sharesById('printerShare-id')->patch($requestBody);


```