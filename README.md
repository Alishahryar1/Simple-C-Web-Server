# Simple-Web-Server

## Introduction
**Simple-Web-Server** is a highly efficient, multithreaded, and platform-independent HTTP and HTTPS server and client library. Developed using modern C++11 and Asio (compatible with both Boost.Asio and standalone Asio), it's designed to provide an easy solution for implementing REST resources in C++ applications.

Check out the advanced [C++ IDE supporting C++11/14/17](https://gitlab.com/cppit/jucipp).

## Features

- **Asynchronous Request Handling:** Efficient management of incoming requests.
- **Thread Pooling:** Optimizes performance in multi-threaded environments.
- **Platform Independence:** Runs seamlessly across different operating systems.
- **HTTPS Support:** Secure communication using the HTTPS protocol.
- **HTTP Persistent Connection:** Maintains connections for HTTP/1.1.
- **Chunked Transfer Encoding:** Supported in the client for efficient data transfer.
- **Configurable Timeouts:** Customizable for `Server::timeout_request` and `Server::timeout_content`.
- **REST Resource Integration:** Easy addition using regex for path matching and anonymous functions.

## Usage

Refer to `http_examples.cpp` or `https_examples.cpp` for practical examples. Pay special attention to the JSON-POST example (utilizing Boost.PropertyTree) and the GET /match/[number] example.

## Dependencies

- **Asio Library:** Either Boost.Asio or standalone Asio.
- **Boost Libraries:** Necessary for compiling examples.
- **OpenSSL Libraries:** Required for HTTPS functionality.

## Compile and Run

### Compilation
Use a C++11 compliant compiler:
```sh
mkdir build
cd build
cmake ..
make
cd ..
