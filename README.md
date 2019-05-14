# bssl-docker
A docker containing the latest bssl command line from BoringSSL

One use case is to run this binary to test TLS1.3 session resumption:

```
docker run --rm -it yegle/bssl client -connect dns.google.com:853 -test-resumption -early-data /dev/null
```
