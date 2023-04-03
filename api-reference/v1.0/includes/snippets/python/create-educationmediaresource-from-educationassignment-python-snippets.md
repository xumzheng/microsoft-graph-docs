---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationAssignmentResource();
requestBody.setDistributeForStudentWork(false);

resource = EducationResource();
resource.set@odatatype('microsoft.graph.educationMediaResource');

resource.setDisplayName('homework example.PNG');

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RMUWOKAGSJZ6BHINJVKNMOOJABF', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


result = await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').resources().post(requestBody);


```