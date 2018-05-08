# NGINX with SPIFFE support
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdrrt%2Fspiffe-nginx.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdrrt%2Fspiffe-nginx?ref=badge_shield)


This version of NGINX Open Source interacts with the SPIFFE Workload API to request and use certificates for mTLS.

Based on configured SPIFFE IDs, it can accept or reject connections.

## Building

Building is best done with the included Dockerfile and Makefile:

* `make container` - builds the compilation container, including depdancies configured in `vendor.sh`
* `make configure` - runs the `./configure` process for nginx, as specified in `build.sh`
* `make` - builds the nginx binary and copies the results to the top level repo directory
* `make clean` - cleans the nginx build
* `make shell` - launches a shell in the build container



## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdrrt%2Fspiffe-nginx.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdrrt%2Fspiffe-nginx?ref=badge_large)