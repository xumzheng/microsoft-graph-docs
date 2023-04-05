---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSubmissionResource()
resource = EducationResource()
resource.setDisplayName('_FTP_EDC-61424749-250820211136.pdf')

resource.set@odatatype('#microsoft.graph.educationFileResource')

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)


result = await client.education_classesby_id('educationClass-id')_assignmentsby_id('educationAssignment-id')_submissionsby_id('educationSubmission-id')_resources.post(request_body)


```