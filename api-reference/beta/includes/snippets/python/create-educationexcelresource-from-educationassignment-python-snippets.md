---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EducationAssignmentResource();
requestBody.setDistributeForStudentWork(false);

resource = EducationResource();
resource.set@odatatype('microsoft.graph.educationExcelResource');

resource.setDisplayName('Graph Doc pages.xlsx');

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').resources().post(requestBody);


```