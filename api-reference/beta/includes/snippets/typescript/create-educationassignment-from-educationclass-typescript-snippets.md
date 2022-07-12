---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationAssignment = {
	dueDateTime : new Date("2021-09-07T00:00:00Z"),
	displayName : "Reading test 09.03 #4",
	instructions : {
		contentType : BodyType.Text,
		content : "Read chapter 4",
	},
	grading : {
		"@odata.type" : "#microsoft.graph.educationAssignmentGradeType",
		additionalData : {
			maxPoints : 50,
		},
	},
	assignTo : {
		"@odata.type" : "#microsoft.graph.educationAssignmentGradeType",
	},
	status : EducationAssignmentStatus.Draft,
	allowStudentsToAddResourcesToSubmission : true,
};

const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignments.post(requestBody);
}


```