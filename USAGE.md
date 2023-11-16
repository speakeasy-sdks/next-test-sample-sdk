<!-- Start SDK Example Usage -->
```go
package main

import (
	"context"
	nexttestsamplesdk "github.com/speakeasy-sdks/next-test-sample-sdk"
	"log"
	"net/http"
)

func main() {
	s := nexttestsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}

	if res.StatusCode == http.StatusOK {
		// handle response
	}
}

```
<!-- End SDK Example Usage -->