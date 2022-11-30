---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Search

$params = @{
	DisplayName = "DNN"
	StandsFor = "Deep Neural Network"
	Description = "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
	WebUrl = "http://microsoft.com/deep-neural-network"
	State = "draft"
}

New-MgBetaSearchAcronym -BodyParameter $params

```