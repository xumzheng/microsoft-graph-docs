---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationAssignmentResource()
request_body.distributeForStudentWork = false

resource = EducationResource()
resource.displayName = 'Where the Wonders of Learning Never Cease | Wonderopolis'

resource.@odatatype = '#microsoft.graph.educationLinkResource'

additionalData = [
'link' => 'https://wonderopolis.org/', 
'thumbnailPreviewUrl' => 		null,
];
resource.additionaldata(additionalData)



request_body.resource = resource



result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').resources.post(request_body = request_body)


```