---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewReferenceCreate()
odataId := "https://graph.microsoft.com/beta/directoryObjects/{id}"
requestBody.SetOdataId(&odataId) 

graphClient.Groups().ByGroupId("group-id").Members().Ref().Post(context.Background(), requestBody, nil)


```