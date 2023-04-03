---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessReviewStage();
requestBody.set@odatatype('#microsoft.graph.accessReviewStage');

reviewersAccessReviewReviewerScope1 = AccessReviewReviewerScope();
reviewersAccessReviewReviewerScope1.setQuery('/users/1ed8ac56-4827-4733-8f80-86adc2e67db5');

reviewersAccessReviewReviewerScope1.setQueryType('MicrosoftGraph');


reviewersArray []= reviewersAccessReviewReviewerScope1;
requestBody.setReviewers(reviewersArray);


fallbackReviewersAccessReviewReviewerScope1 = AccessReviewReviewerScope();
fallbackReviewersAccessReviewReviewerScope1.setQuery('/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e');

fallbackReviewersAccessReviewReviewerScope1.setQueryType('MicrosoftGraph');


fallbackReviewersArray []= fallbackReviewersAccessReviewReviewerScope1;
fallbackReviewersAccessReviewReviewerScope2 = AccessReviewReviewerScope();
fallbackReviewersAccessReviewReviewerScope2.setQuery('/users/1ed8ac56-4827-4733-8f80-86adc2e67db5');

fallbackReviewersAccessReviewReviewerScope2.setQueryType('MicrosoftGraph');


fallbackReviewersArray []= fallbackReviewersAccessReviewReviewerScope2;
requestBody.setFallbackReviewers(fallbackReviewersArray);




result = awaitclient.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instancesById('accessReviewInstance-id').stagesById('accessReviewStage-id').patch(requestBody);


```