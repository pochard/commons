# commons
common tool functions for Golang. The package randstr is to create a random string with a specified length.

Import it in your program as:
```go
      import "github.com/pochard/commons"
```

## API
### pakcage randstr
	func Random(n int, chars string) string
	func RandomAlphanumeric(n int) string
	func RandomAlphabetic(n int) string
	func RandomNumeric(n int) string 
	func RandomAscii(n int) string

	
## Example
```go
package main

import (
        "github.com/pochard/commons/randstr"
)

func main() {
        //letters + numbers
        println(randstr.RandomAlphanumeric(17))
        //letters
        println(randstr.RandomAlphabetic(17))
        //numbers
        println(randstr.RandomNumeric(17))
        //letters + numbers + other visible ascii chars
        println(randstr.RandomAscii(17))
        //specified chars
        println(randstr.Random(17, "abcde123"))
}

```
