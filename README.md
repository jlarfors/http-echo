# http-echo

Forked from <https://github.com/hashicorp/http-echo>

=========

HTTP Echo is a small go web server that serves the contents it was started with
as an HTML page.

The default port is 5678, but this is configurable via the `-listen` flag or `ECHO_TEXT` environment variable:

```bash
# Using -listen flag
http-echo -listen=:8080 -text="hello world"

# Using ECHO_TEXT env var
ECHO_TEXT="hello world" http-echo -listen=:8080
```

Then visit <http://localhost:8080/> in your browser.
