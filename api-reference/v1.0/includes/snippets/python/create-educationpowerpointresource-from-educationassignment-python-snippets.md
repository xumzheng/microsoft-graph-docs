---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationAssignmentResource();
requestBody.setDistributeForStudentWork(false);

resource = EducationResource();
resource.set@odatatype('microsoft.graph.educationPowerPointResource');

resource.setDisplayName('state diagram.pptx');

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


result = await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').resources().post(requestBody);


```