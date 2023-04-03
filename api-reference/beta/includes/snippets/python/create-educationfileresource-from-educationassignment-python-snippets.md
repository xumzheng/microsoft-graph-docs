---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationAssignmentResource();
requestBody.setDistributeForStudentWork(false);

resource = EducationResource();
resource.setDisplayName('article.pdf');

resource.set@odatatype('#microsoft.graph.educationFileResource');

additionalData = [
'file' => resource = File();
		resource.setOdataid('https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RPHKSP6THE4ORD2RQAR6MQLF26G');


resource.setFile($file);

];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').resources().post(requestBody);


```