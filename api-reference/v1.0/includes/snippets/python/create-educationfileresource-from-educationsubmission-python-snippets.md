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
'fileUrl' => 'https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXodJYOAkI7rTLhw7ME_e42J/items/01QTY63RL45XVPGDBRW5FLDR62Z5TCMGG3', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)

request_config = ResourcesRequestBuilderPostRequestConfiguration(
request_config = ResourcesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').resources.post(request_body, headers=)


```