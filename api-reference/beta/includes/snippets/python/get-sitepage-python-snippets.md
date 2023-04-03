---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = SitePageRequestBuilderGetRequestConfiguration();

queryParameters = SitePageRequestBuilderGetQueryParameters();
queryParameters.select = ["id","title"];
queryParameters.expand = ["webparts"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.sitesById('site-id').pagesById('sitePage-id').get(requestConfiguration);


```