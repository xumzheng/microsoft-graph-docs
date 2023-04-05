---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSubmissionResource()
resource = EducationResource()
resource.setDisplayName('Wikipedia')

resource.set@odatatype('#microsoft.graph.educationLinkResource')

additionalData = [
'link' => 'https://en.wikipedia.org/wiki/Main_Page', 
];
resource.setAdditionalData(additionalData)



request_body.setResource($resource)


result = await client.education.classes._by_id('educationClass-id').assignments._by_id('educationAssignment-id').submissions._by_id('educationSubmission-id').resources.post(request_body)


```