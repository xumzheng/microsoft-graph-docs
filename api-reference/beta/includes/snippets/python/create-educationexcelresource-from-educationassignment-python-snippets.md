---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.setDistributeForStudentWork(false)

resource = EducationResource()
resource.set@odatatype('microsoft.graph.educationExcelResource')

resource.setDisplayName('Graph Doc pages.xlsx')

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)


result = await client.education.classesById('educationClass-id').assignmentsById('educationAssignment-id').resources.post(request_body)


```