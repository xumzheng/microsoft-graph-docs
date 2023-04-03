---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EducationAssignmentResource();
requestBody.setDistributeForStudentWork(false);

resource = EducationResource();
resource.setDisplayName('Where the Wonders of Learning Never Cease | Wonderopolis');

resource.set@odatatype('#microsoft.graph.educationLinkResource');

additionalData = [
'link' => 'https://wonderopolis.org/', 
'thumbnailPreviewUrl' => 		null,
];
resource.setAdditionalData(additionalData);



requestBody.setResource($resource);


requestResult = graphServiceClient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').resources().post(requestBody);


```