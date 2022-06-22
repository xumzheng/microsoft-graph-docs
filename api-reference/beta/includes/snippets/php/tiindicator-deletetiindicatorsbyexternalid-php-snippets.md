---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValueRequestBody();


$requestRequestBody->setValue( [
'externalId-value1','externalId-value2',],
$result =  $graphClient->security()->tiIndicators()->deleteTiIndicatorsByExternalId()->post($requestRequestBody);


```