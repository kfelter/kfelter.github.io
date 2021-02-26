# Kyle Felter

Contact: kylerfelter@gmail.com

Resume: [pdf](/resume.pdf) [MD](/resume.md)

## Projects
* [tolerance](https://github.com/kfelter/tolerance) - fault tolerant math operations in golang inspired by spacex
* [apguard](https://github.com/kfelter/apguard) - distributed proxy that acts as a rate limiter for downstream http services
* [c++ arduino game](https://github.com/kfelter/ard-memory-game) - memory game deployed on an arduino
* [react/python/serverless](https://github.com/kfelter/CoreColor) - color picking and voting app deployed using aws s3 and aws lambda
* [go concurrecny model](https://github.com/kfelter/go_concurrency_example) - examples of how to use channels and go routines to design concurrent go code
* [Caverunner](https://filebox.ece.vt.edu/~mhsiao/video_game/proj2016/kyle_felter.html) - While creating this game I had to think about limitations of graphics within the browser and how to make the code efficient enough to run on most computers.
* [Path finding Hokie](https://filebox.ece.vt.edu/~mhsiao/video_game/proj2016/Proj8_4.html) - fun game that uses BFS to move a Hokie around in a maze.
* [Basketball Game](https://filebox.ece.vt.edu/~mhsiao/video_game/proj2016/Proj5_4.html) - physics simulation in javascript used to make a small basketball game.

## Code Samples

Simple Hello World in Go

```go
package main

import "fmt"

func main() {
  fmt.Println("Hello, World!")
}
```

Simple golang http service

```go
package main

import (
	"flag"
	"io/ioutil"
	"log"
	"net/http"
)

var (
	p = flag.String("port", "80", "server port")
)

func main() {
	http.HandleFunc("/", greetHandler)
	panic(http.ListenAndServe(":"+*p, nil))
}

func greetHandler(w http.ResponseWriter, req *http.Request) {
	log.Printf("Hello there %s\n", req.RemoteAddr)
	ioutil.ReadAll(req.Body)
	req.Body.Close()
	w.WriteHeader(http.StatusOK)
	w.Write([]byte(`Hello there` + "\n"))
}
```

Simple go reverse proxy

```go
package main

import (
	"flag"
	"log"
	"net/http"
	"net/http/httputil"
	"net/url"
)

var (
	p      = flag.String("port", "80", "port")
	origin = flag.String("origin", "", "url to be proxied")
)

func main() {
	flag.Parse()

	parsedURL, _ := url.Parse(*origin)

	proxy := httputil.NewSingleHostReverseProxy(parsedURL)

	http.HandleFunc("/", proxy.ServeHTTP)

	log.Fatal(http.ListenAndServe(":"+*p, nil))
}
```

