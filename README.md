
```
package main

import (
	"log"

	"github.com/monitorapp-aicc/logger"
)

func main() {
	log.SetFlags(log.LstdFlags | log.Lshortfile)
	l := logger.Logger{
		Directory: "logs",
		Prefix:    "feed_server",
	}
	l.InitStandardLogger(logger.FILE)
	log.Println("log test")
}
```
