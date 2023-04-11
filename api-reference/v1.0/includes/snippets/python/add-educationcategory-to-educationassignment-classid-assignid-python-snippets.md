---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = RefRequestBuilderDeleteRequestConfiguration(
)


await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').categories_by_id('educationCategory-id').ref.delete()


```