---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationSubmissionResource();
resource = EducationResource();
resource.setDisplayName('category.jpg');

resource.set@odatatype('#microsoft.graph.educationMediaResource');

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RK2WLKUUBAA4ZBKXNBL6QFC2TKG', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


result = await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').resources().post(requestBody);


```