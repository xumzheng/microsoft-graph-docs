---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PrinterShareRequestBuilderGetRequestConfiguration();

queryParameters = PrinterShareRequestBuilderGetQueryParameters();
queryParameters.select = ["id","displayName","capabilities"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.print().sharesById('printerShare-id').get(requestConfiguration);


```