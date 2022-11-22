---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.Governance

Get-MgIdentityGovernanceLifecycleWorkflowRunUserProcessingResult -WorkflowId $workflowId -RunId $runId -Property "id,failedTasksCount,processingStatus,totalTasksCount,totalUnprocessedTasksCount,subject" 

```