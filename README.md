# building image
updated to make for solo-io
```bash
make linux/arm64 #-- based off the architecture you want to build
make docker-build/alpine
```
get the tag name and push it
then push the image to `gcr.io/solo-test-236622/http-echo`
Metadata about this makefile and position


http-echo
=========
HTTP Echo is a small go web server that serves the contents it was started with
as an HTML page.

The default port is 5678, but this is configurable via the `-listen` flag:

```
http-echo -listen=:8080 -text="hello world"
```

Then visit http://localhost:8080/ in your browser.
