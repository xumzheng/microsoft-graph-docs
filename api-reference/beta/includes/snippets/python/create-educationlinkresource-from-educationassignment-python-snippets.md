---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.setDistributeForStudentWork(false)

resource = EducationResource()
resource.setDisplayName('Where the Wonders of Learning Never Cease | Wonderopolis')

resource.set@odatatype('#microsoft.graph.educationLinkResource')

additionalData = [
'link' => 'https://wonderopolis.org/', 
'thumbnailPreviewUrl' => 		null,
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').resources.post(request_body, headers=)


```