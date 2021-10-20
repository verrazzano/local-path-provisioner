FROM ghcr.io/oracle/oraclelinux:7-slim
RUN yum update -y
COPY bin/local-path-provisioner /usr/bin/
COPY LICENSE README.md.in THIRD_PARTY_LICENSES.txt SECURITY.md /license/
CMD ["local-path-provisioner"]
