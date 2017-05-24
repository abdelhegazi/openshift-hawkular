#FROM docker.io/fabric8/s2i-java:1.3.6
FROM fabric8/fabric8-java

ENV APM_VERSION=0.14.4.Final
ENV APM_AGENT=/libs/hawkular-apm-agent.jar

ADD https://github.com/hawkular/hawkular-apm/releases/download/$APM_VERSION/hawkular-apm-agent.jar $APM_AGENT


# Temporary switch to root
USER root

RUN chmod 444 /libs/hawkular-apm-agent.jar

# S2I requires a numeric, non-0 UID. This is the UID for the jboss user in the base image
USER 185
