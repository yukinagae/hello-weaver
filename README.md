# hello-weaver

see: [Service Weaver](https://serviceweaver.dev/docs.html)


## Requirements

- [Go](https://go.dev/doc/install)

```bash
$ which go                                     
/usr/local/go/bin/go
$ go version
go version go1.20.1 darwin/amd64
```

## Run

```bash
$ cd hello-weaver
$ go mod tidy
$ go run .
hello listener available on 127.0.0.1:12345
╭───────────────────────────────────────────────────╮
│ app        : hello                                │
│ deployment : a5d86fb7-bf35-49c8-82c1-b7247293f3d2 │
╰───────────────────────────────────────────────────╯
```

Use curl to check it works!

```bash
$ curl "http://localhost:12345/hello?name=Weaver"
Hello, Weaver!
```
