---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new PrinterRequestBuilderGetRequestConfiguration();

$queryParameters = new PrinterRequestBuilderGetQueryParameters();
$queryParameters->select = ["id","displayName","capabilities"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->print()->printersById('printer-id')->get($requestConfiguration);


```