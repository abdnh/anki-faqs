# Anki must be able to connect to a local port

When Anki 2.1 starts up, it listens on a port on localhost for requests from the user interface. If you have a proxy server configured on your machine, please go into your proxy settings and make sure that "bypass proxy server for local addresses" is enabled - otherwise Anki's user interface will have its local communication redirected through the proxy, which will prevent Anki from functioning.

More info: <https://superuser.com/a/261434>

This problem may also occur if you have a firewall running on your machine that blocks local connections, or are using a VPN that is incorrectly redirecting local traffic.
