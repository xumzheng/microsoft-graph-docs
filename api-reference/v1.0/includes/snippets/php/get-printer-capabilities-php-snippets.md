---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PrinterRequestBuilderGetRequestConfiguration();

$queryParameters = new PrinterRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,displayName,capabilities';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->print()->printersById('printer-id')->get($requestConfiguration);


```