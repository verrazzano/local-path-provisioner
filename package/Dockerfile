FROM ghcr.io/oracle/oraclelinux:7-slim
RUN yum update -y && \
    yum clean all && \
    rm -rf /var/cache/yum

COPY bin/local-path-provisioner /usr/bin/
COPY LICENSE README.md THIRD_PARTY_LICENSES.txt SECURITY.md /licenses/
CMD ["local-path-provisioner"]
