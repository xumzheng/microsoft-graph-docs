---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationSubmissionResource();
resource = EducationResource();
resource.set@odatatype('#microsoft.graph.educationPowerPointResource');

resource.setDisplayName('state diagram.pptx');

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RN3MHWWM7BNXJD2UD5OMRFEDKN2', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').resources().post(requestBody);


```