# python-proxy
https://code.google.com/archive/p/python-proxy/

At this point this proxy is an Elie Proxy.
Supports HTTP methods:
 - OPTIONS;
 - GET;
 - HEAD;
 - POST;
 - PUT;
 - DELETE;
 - TRACE;
 - CONCENT.
Supports:
 - Client connections in IPv4 or IPv6;
 - IPv4 and IPv6 target connections;
 - Connections all type of TCP (CONNECT tunneling) data transmission,
     Eg SSL connections, such as HTTPS.
To do:
 - Verify that the input coming from the client is correct;
   - Send the appropriate HTTP errors if not, or simply break the connection;
 - Create an error manager;
 - Create error log file;
 - Place exceptions in places where errors are expected,
     E.g., sockets and files;
 - Review everything and improve the structure of programming and put appropriate names in the
     Variables and methods;
 - Discuss the program decently;
 Doc Strings.
Future features:
 - Add anonymous and transparent proxy functionality;
 - Support FTP ?.
(!) Caution The following only works on non-CONNECT connections, for these the
 Proxy is always Elite.
What is the difference between an Elite, Anonymous and Transparent proxy?
 - An elite proxy is totally anonymous, the receiving server can not have
     Knowledge of the existence of the proxy and does not receive the IP address of the client;
 - When an anonymous proxy is used the server knows that the client is using a
     Proxy but does not know the IP address of the client;
     The HTTP header "Proxy-agent" is sent.
 - A transparent proxy provides the server with the client IP and information that
     If you are using a proxy.
     The HTTP headers "Proxy-agent" and "HTTP_X_FORWARDED_FOR" are sent.
