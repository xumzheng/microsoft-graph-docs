---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationSubmissionResource();
resource = EducationResource();
resource.setDisplayName('Wikipedia');

resource.set@odatatype('#microsoft.graph.educationLinkResource');

additionalData = [
'link' => 'https://en.wikipedia.org/wiki/Main_Page', 
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


result = await client.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').resources().post(requestBody);


```