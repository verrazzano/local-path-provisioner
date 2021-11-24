# Copyright (C) 2021, Oracle and/or its affiliates.
# Licensed under the Universal Permissive License v 1.0 as shown at https://oss.oracle.com/licenses/upl.

FROM ghcr.io/oracle/oraclelinux:7-slim
RUN yum update -y && \
    yum clean all && \
    rm -rf /var/cache/yum

COPY bin/local-path-provisioner /usr/bin/
COPY LICENSE README.md THIRD_PARTY_LICENSES.txt SECURITY.md /licenses/
CMD ["local-path-provisioner"]
