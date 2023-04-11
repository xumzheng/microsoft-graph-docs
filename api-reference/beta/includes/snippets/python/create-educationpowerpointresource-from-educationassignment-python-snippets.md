---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.distributeForStudentWork = false

resource = EducationResource()
resource.@odatatype = 'microsoft.graph.educationPowerPointResource'

resource.displayName = 'state diagram.pptx'

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ', 
];
resource.additionaldata(additionalData)



request_body.resource = resource


request_configuration = ResourcesRequestBuilderPostRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').resources.post(request_body = request_body)


```