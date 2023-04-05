---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.setDistributeForStudentWork(false)

resource = EducationResource()
resource.set@odatatype('microsoft.graph.educationPowerPointResource')

resource.setDisplayName('state diagram.pptx')

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)


result = await client.education.classes._by_id('educationClass-id').assignments._by_id('educationAssignment-id').resources.post(request_body)


```