# http-echo

=========

HTTP Echo is a small go web server that serves the contents it was started with
as an HTML page.

## Install

### Homebrew

```bash
brew install verifa/tap/http-echo
```

### Docker

```bash
docker pull verifa/http-echo
```

## Usage

The default port is 5678, but this is configurable via the `-listen` flag.

```bash
# Using -listen flag
http-echo -listen=:8080 -text="hello world"

# Using ECHO_TEXT env var
ECHO_TEXT="hello world" http-echo -listen=:8080

# Using Docker
docker run -e ECHO_TEXT='hello world!' -p 8080:8080 verifa/http-echo -listen :8080
```

Then visit <http://localhost:8080/> in your browser.

=========

Forked from <https://github.com/hashicorp/http-echo>
