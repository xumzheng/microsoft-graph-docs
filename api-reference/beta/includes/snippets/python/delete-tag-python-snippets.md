---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = TagRequestBuilderDeleteRequestConfiguration();

queryParameters = TagRequestBuilderDeleteQueryParameters();
queryParameters.forcedelete = true;

requestConfiguration.queryParameters = queryParameters;


graphServiceClient.compliance().ediscovery().casesById('case-id').tagsById('tag-id').delete(requestConfiguration);


```