---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationSubmissionResource()
resource = EducationResource()
resource.displayName = 'Wikipedia'

resource.@odatatype = '#microsoft.graph.educationLinkResource'

additionalData = [
'link' => 'https://en.wikipedia.org/wiki/Main_Page', 
];
resource.additionaldata(additionalData)



request_body.resource = resource


request_configuration = ResourcesRequestBuilderPostRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').resources.post(request_body = request_body)


```