# logrus-gce
Google Cloud Engine Logging Formatter for Logrus

Forked from https://github.com/znly/logrus-gce for use with the Sharescape stack. 

## How to use
```golang
package main

import (
	log "github.com/Sirupsen/logrus"
    logrusgce "github.com/znly/logrus-gce"
)

func main() {
    log.SetFormatter(logrusgce.NewGCEFormatter(true))
    log.WithField("myfield", "myvalue").Info("hey")
}
```
