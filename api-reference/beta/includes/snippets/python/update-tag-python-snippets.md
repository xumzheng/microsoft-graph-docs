---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Tag();
$requestBody->setDescription('This is an updated description.');



$requestResult = $graphServiceClient->compliance()->ediscovery()->casesById('case-id')->tagsById('tag-id')->patch($requestBody);


```