# [neva.li](https://neva.li/)

This repository contains the root of [my website](https://neva.li). Its
contents consist mostly of common, static files.

## Structure

As with any Github Pages-hosted domain, each individual repository may
have its own set of web resources. Of particular interest is
[my notebook](https://neva.li/notebook) ([source repository](https://github.com/nevali/notebook)),
which is [generated automatically](https://travis-ci.org/nevali/notebook)
from [the Github Wiki](https://github.com/nevali/notebook/wiki).

## How the site is served

Because Github Pages can't serve via TLS with a custom domain, DNS is
configured to point to a different host which then proxies requests back
to the Github-hosted resources.

Any files which exist within the document root on the web host are served
directly, but the aim is to reduce that to zero and have everything hosted
via Github and built with Travis where needed.
