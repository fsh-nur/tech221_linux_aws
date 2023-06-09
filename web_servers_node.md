# Webservers, Node.js, NPM


## How do Webservers work?

Computer programs that dispense the web page when they are requested using the web client. The machines where these programs run are called servers. They can be downloaded onto a computer system. They will receive a request from a web client access it from a storage location and send it back.

This can be done is 4 main steps:
1. Obtaining the IP Address from the domain name
2. Browser requests the full URL
3. The web server responds to request
4. The browser displays the web page

## Node.js and Use Cases

Node.js is a server-side runtime environment based on the event-driven programming language and has non-blocking I/O capabilities.  Use cases are: building webservers, command-line tools, desktop applications

## What are the dependencies of Nodejs?

Nodejs has a number of dependecies including libraries and tools: including OpenSSL, npm, z lib and gyp:
- Openssl: OpenSSL is used extensively in both the tls and crypto modules. It provides battle-tested implementations of many cryptographic functions that the modern web relies on for security.
- NPM:Node.js is all about modularity, and with that comes the need for a quality package manager; for this purpose, npm was made. With npm comes the largest selection of community-created packages of any programming ecosystem, which makes building Node.js apps quick and easy.
- zlib: For fast compression and decompression, Node.js relies on the industry-standard zlib library, also known for its use in gzip and libpng. Node.js uses zlib to create sync, async and streaming compression and decompression interfaces.
- gyp:The build system is handled by gyp, a python-based project generator copied from V8. It can generate project files for use with build systems across many platforms. Node.js requires a build system because large parts of it — and its dependencies — are written in languages that require compilatio

## What is a reverse proxy?

A reverse proxy is a server that sits in front of one or more web servers, intercepting requests from clients. 
A reverse proxy works by intercepting a request from a client, performing some action on the request, then sending the request on to the appropriate origin server in the network. The origin server’s response then travels back through the reverse proxy, giving the impression to clients that the proxy server handled the request on its own.
