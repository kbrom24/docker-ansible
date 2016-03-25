FROM ubuntu:trusty
MAINTAINER lorin@ansiblebook.com
# Based on the Digital Ocean tutorial: http://bit.ly/1qJ8CXP
# Update the default application repository sources list
RUN apt-get update
# Install Memcached
RUN apt-get install -y memcached

# Port to expose (default: 11211)
EXPOSE 11211
# Default Memcached run command arguments
CMD ["-m", "128"]
# Set the user to run Memcached daemon
USER daemon
# Set the entrypoint to memcached binary
ENTRYPOINT memcached
