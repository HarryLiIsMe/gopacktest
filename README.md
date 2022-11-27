# GoPackTest
## Test go package publish use
## Go use code
```
package main

import (
	"fmt"
	"github.com/harryliisme/gopacktest/test"
)

func main() {
	fmt.Println("go pack test use")
	test.Test()
}
```

## Go mod file(go.mod)
```
require github.com/harryliisme/gopacktest git_tag(no release flag)/version
```

## Go use command
### The github do not really remove any tag afther author remove its on github repo, and just hide the removed tags by author. 
### so go get\go mod tidy still download the uploaded tags when author remove its on github.
```
go clean
go mod tidy
go get 
go mod download
go build
```