# Clai
**clai** is a CLI tool for interacting with LLM APIs (specifically targetting ollama).

## Building
1. Make sure you got Golang 1.25.3 installed.
2. Run the following commands:
```bash
[[ ! -d "./bin" ]] && mkdir ./bin
#go mod tidy
go generate ./...
#go mod tidy
#go vet ./...
go build -v -x -o bin/clai cmd/cli/main.go
```
**or**

2. Run the following command:
```bash
./build
```

## Running
1. Make sure you build as per above.
2. Run the following commands:
```bash
chmod +x ./bin/clai
./bin/clai
```
**or**

2. Run the following command:
```bash
./run
```

# License
**clai** is released under the [LGPL-2.1 License](https://github.com/Ktnuity/clai/blob/master/COPYING).
