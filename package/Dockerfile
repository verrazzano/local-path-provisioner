FROM ghcr.io/oracle/oraclelinux:7-slim
RUN yum update -y
COPY bin/local-path-provisioner /usr/bin/
CMD ["local-path-provisioner"]
