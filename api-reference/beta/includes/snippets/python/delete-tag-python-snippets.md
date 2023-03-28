---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new TagRequestBuilderDeleteRequestConfiguration();

$queryParameters = new TagRequestBuilderDeleteQueryParameters();
$queryParameters.forcedelete = true;

$requestConfiguration.queryParameters = $queryParameters;


$graphServiceClient.compliance().ediscovery().casesById('case-id').tagsById('tag-id').delete($requestConfiguration);


```