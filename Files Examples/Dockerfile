ARG VERSION=1.2.0
#Use this repository for an standard costumer token
ARG BASE=bonitasoft.jfrog.io/docker/bonita-ui-builder
#Use this repository for an internal Bonita token
#ARG BASE=bonitasoft.jfrog.io/docker-release/bonita-ui-builder

FROM ${BASE}:${VERSION}

# Argument for the folder location on the host where exported JSON applications are stored
ARG WORKSPACE=./workspace/

# Make sure that the dev mode is disabled
ENV BONITA_DEV_MODE=false

# Copy JSON applications inside an internal folder to be imported at startup
COPY ${WORKSPACE} /opt/appsmith/workspace/applications/

EXPOSE 80
EXPOSE 443
ENTRYPOINT [ "/opt/appsmith/entrypoint.sh" ]
HEALTHCHECK --interval=15s --timeout=15s --start-period=45s CMD "/opt/appsmith/healthcheck.sh"
CMD ["/usr/bin/supervisord", "-n"]