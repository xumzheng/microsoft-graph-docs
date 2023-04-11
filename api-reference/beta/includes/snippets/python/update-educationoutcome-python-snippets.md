---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.@odatatype = '#microsoft.graph.educationRubricOutcome'

additionalData = [
'rubricQualityFeedback' => rubricQualityFeedback1 = ()
		rubricQualityFeedback1.qualityId = '9a145aa8-f3d9-43a1-8f77-5387ff0693f2'

rubricQualityFeedback1Feedback = Feedback()
		rubricQualityFeedback1Feedback.content = 'This is feedback specific to the first quality of the rubric.'

		rubricQualityFeedback1Feedback.contentType = 'text'


rubricQualityFeedback1.feedback = rubricQualityFeedback1Feedback

rubricQualityFeedbackArray []= rubricQualityFeedback1;
rubricQualityFeedback2 = ()
		rubricQualityFeedback2.qualityId = 'd2331fb2-2761-402e-8de6-93e0afaa076e'

rubricQualityFeedback2Feedback = Feedback()
		rubricQualityFeedback2Feedback.content = 'This is feedback specific to the second quality of the rubric.'

		rubricQualityFeedback2Feedback.contentType = 'text'


rubricQualityFeedback2.feedback = rubricQualityFeedback2Feedback

rubricQualityFeedbackArray []= rubricQualityFeedback2;
request_body.rubricqualityfeedback(rubricQualityFeedbackArray)


'rubricQualitySelectedLevels' => rubricQualitySelectedLevels1 = ()
	rubricQualitySelectedLevels1.qualityId = '9a145aa8-f3d9-43a1-8f77-5387ff0693f2'

	rubricQualitySelectedLevels1.columnId = '4fb17a1d-5681-46c2-a295-4e305c3eae23'


rubricQualitySelectedLevelsArray []= rubricQualitySelectedLevels1;
rubricQualitySelectedLevels2 = ()
	rubricQualitySelectedLevels2.qualityId = 'd2331fb2-2761-402e-8de6-93e0afaa076e'

	rubricQualitySelectedLevels2.columnId = 'aac076bf-51ba-48c5-a2e0-ee235b0b9740'


rubricQualitySelectedLevelsArray []= rubricQualitySelectedLevels2;
request_body.rubricqualityselectedlevels(rubricQualitySelectedLevelsArray)


];
request_body.additionaldata(additionalData)




request_configuration = EducationOutcomeRequestBuilderPatchRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes_by_id('educationOutcome-id').patch(request_body = request_body)


```