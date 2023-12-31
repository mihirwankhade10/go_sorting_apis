# Sorting APIs in Go

## Overview
This project implements a Go server with two endpoints for sorting arrays sequentially and concurrently. It provides a demonstration of sequential and concurrent processing, measuring the time taken for each sorting method.

## Features
- **Sequential Sorting:** Endpoint to sequentially sort input arrays.
- **Concurrent Sorting:** Endpoint to concurrently sort input arrays using Go's concurrency features.
- **Performance Measurement:** Measures the time taken to sort arrays in nanoseconds.
- **Dockerization:** The project is containerized using Docker.

## API working Screenshots

- http://localhost:8000/process-single
<img width="960" alt="single-processing-sc1" src="https://github.com/mihirwankhade10/go_sorting_apis/assets/87888969/950c4f28-c5a4-4e63-9b2d-9a664867fa11">

- http://localhost:8000/process-concurrent
<img width="960" alt="concurrent-processing-sc1" src="https://github.com/mihirwankhade10/go_sorting_apis/assets/87888969/d958ab40-41f8-49c1-9833-a09e85361e2c">

## Getting Started
### Prerequisites
- [Go](https://golang.org/dl/) installed on your machine.
- [Docker](https://docs.docker.com/get-docker/) installed (for Dockerization).

### Installation
```bash
# Clone the repository
git clone https://github.com/mihirwankhade10/go_sorting_apis.git
cd sorting-apis-go

# Build the Go application
go build -o main .

# Run the application
./main
```
## Dockerization
### Build Docker image
docker build -t aegon10/sortingapis:latest .

### Run Docker container
docker run -p 8000:8000 aegon10/sortingapis:latest


Make sure to replace the placeholders like `aegon10` and `sorting-apis-go` with your actual Docker username and repository name.
