# HTTP2

## Description

This very simple app demonstrates using Jetty's HTTP2 capabilties.

## Usage

1. Set the appropriate ALPN-Boot version within `project.clj` based on your JDK Version
2. Start the application: `lein run`
3. Go to [localhost:8080](http://localhost:8080/) to see an HTTP 1.1 message.
4. Go to [localhost:8443](http://localhost:8443/) to see an HTTP2 message.

You can also use an HTTP2-enabled command line client:

1. Direct HTTP2 clear-text request: `nghttp -v http://localhost:8080/`
2. Upgrade an HTTP/1.1 request to a clear-text HTTP2 request: `nghttp -vu http://localhost:8080/`

License
-------
Copyright 2013 Relevance, Inc.
Copyright 2015 Cognitect, Inc.

The use and distribution terms for this software are covered by the
Eclipse Public License 1.0 (http://opensource.org/licenses/eclipse-1.0)
which can be found in the file epl-v10.html at the root of this distribution.

By using this software in any fashion, you are agreeing to be bound by
the terms of this license.

You must not remove this notice, or any other, from this software.
