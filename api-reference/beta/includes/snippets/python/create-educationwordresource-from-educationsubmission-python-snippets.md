---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSubmissionResource()
resource = EducationResource()
resource.set@odatatype('microsoft.graph.educationWordResource')

resource.setDisplayName('Report.docx')

additionalData = [
'fileUrl' => 'https://graph.microsoft.com/beta/drives/b!DPA6q59Tw0mtgmyXRUmrQRqBZTesG-lMkl1cBmvvMeUEWrOk89nKRpUEr4ZhNYBc/items/016XPCQEELISJB7NVNVBAK7V4UIF6Q27U2', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)

request_config = ResourcesRequestBuilderPostRequestConfiguration(
request_config = ResourcesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').resources.post(request_body, headers=)


```