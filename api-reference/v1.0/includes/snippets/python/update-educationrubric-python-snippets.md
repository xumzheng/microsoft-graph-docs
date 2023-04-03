---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationRubric();
requestBody.setDisplayName('Example Credit Rubric after display name patch');



result = await client.education().me().rubricsById('educationRubric-id').patch(requestBody);


```