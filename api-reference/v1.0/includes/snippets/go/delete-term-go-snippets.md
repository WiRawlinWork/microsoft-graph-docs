---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Sites().BySiteId("site-id").TermStore().Sets().BySetId("set-id").Terms().ByTermId("term-id").Delete(context.Background(), nil)


```