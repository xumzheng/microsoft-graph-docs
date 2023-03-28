---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MailFolder();
$requestBody->set@odatatype('microsoft.graph.mailSearchFolder');

$additionalData = [
'filterQuery' => 'contains(subject, \'Analytics\')', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->me()->mailFoldersById('mailFolder-id')->patch($requestBody);


```