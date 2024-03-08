<!-- Start SDK Example Usage [usage] -->
```go
package main

import (
	"context"
	nexttestsamplesdk "github.com/speakeasy-sdks/next-test-sample-sdk"
	"log"
)

func main() {
	s := nexttestsamplesdk.New()

	ctx := context.Background()
	res, err := s.Pets.CreatePets(ctx)
	if err != nil {
		log.Fatal(err)
	}
	if res != nil {
		// handle response
	}
}

```
<!-- End SDK Example Usage [usage] -->