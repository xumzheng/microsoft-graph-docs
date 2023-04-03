---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EducationAssignmentResource();
requestBody.setDistributeForStudentWork(false);

resource = EducationResource();
resource.set@odatatype('microsoft.graph.educationWordResource');

resource.setDisplayName('Issues and PR in guthub.docx');

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').resources().post(requestBody);


```