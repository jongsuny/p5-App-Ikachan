# NAME

ikachan - IRC message delivery by HTTP

# SYNOPSIS

    # connect to chat.freenode.net
    ikachan -S chat.freenode.net

# OPTIONS

- \-o, --host

    The interface a TCP based server daemon binds to. Default bind address
    is '127.0.0.1'. 

- \-p, --port (default: 4979)

    The port number a TCP based server daemon listens on. Defaults to
    5000\. This option doesn't mean anything if the server does not support
    TCP socket.

- \-S, --Server

    irc server address.

- \-P, --Port (default: 6667)

    irc server port.

- \-K, --Keyword

    irc server password

- \-N, --Nickname

    irc nickname

- \-U, --User

    irc user name

- \-r, --reverse-proxy

    treat X-Forwarded-For as REMOTE\_ADDR if REMOTE\_ADDR match this argument.

    see [Plack::Middleware::ReverseProxy](http://search.cpan.org/perldoc?Plack::Middleware::ReverseProxy).

- \-i, --interval

    irc post interval. for Excess Flood

- \-R, --reconnect-interval

    interval of reconnect to irc server.
    exit application if interval == 0.

- \-j, --no-post-with-join

    disable to irc message post with channel join

- \-m, --mount

    provide TCP based server daemon with path. Default do nothing.

# AUTHOR

Kazuhiro Osawa <yappo {at} shibuya {dot} pl>

# SEE ALSO

[AnySan::Provider::IRC](http://search.cpan.org/perldoc?AnySan::Provider::IRC), [Twiggy](http://search.cpan.org/perldoc?Twiggy)

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.
