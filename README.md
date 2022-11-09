# ApacheHttpd24Config

Apache httpd2.4 config patch for CNSCC.311-Distributed Systems.

## Prerequisite

- Httpd 2.4 binary release (download it from [here](https://httpd.apache.org/docs/current/platform/windows.html#down))

## Usage

1. Extract httpd 2.4 binaries.
2. Replace configs in `conf` folder with this repository.
3. Edit port number in [httpd.conf](https://github.com/TheCuprum/ApacheHttpd24Config/blob/39d2d670050c5e02a0d70581ec1ee5894d23a84a/conf/httpd.conf#L67) and [http-vhosts.conf]().
4. Add your cluster instances under [`<Proxy balancer://cluster>`](https://github.com/TheCuprum/ApacheHttpd24Config/blob/39d2d670050c5e02a0d70581ec1ee5894d23a84a/conf/extra/httpd-vhosts.conf#L76).
5. Configure other options according to your own need.
6. restart httpd.exe or httpd service.
