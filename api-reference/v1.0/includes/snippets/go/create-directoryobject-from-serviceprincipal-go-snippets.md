---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/models"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.ServicePrincipals().ByServicePrincipalId("servicePrincipal-id").Owners().Ref().Post(context.Background(), requestBody, nil)


```