# Wait for services

Very simple docker that does nothing else that services inside a container respond on a port.

This images contains the famous [wait-for-it](https://github.com/vishnubob/wait-for-it) script (slightly adjusted to alpine) to actually do the checking.

Use the container for flow control outside the container:

```
docker run --rm -it leifg/wait-for -h <service_address> -p <service_port> && <other command>
```
