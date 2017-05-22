### openshift-hawkular

This repo is meant to be  astarter how to use Hawkular module that comes as built-in module within openshift. 
 That tool is in charge of collecting metrics from Docker containers through the Kubernetes interface and storing, aggregating, and visualizing them. The metrics collected are CPU, Memory, Disk, and Network usage. Hawkular offers a “black-box” view of container performance but does not deal with application metrics like service performance or distribution of response time through application layers. For this specific case, the Hawkular community is working on another module called Hawkular APM that provides insight into the way an application executes across multiple (micro) services in a distributed (e.g. cloud) environment. Hawkular APM supports agent-based instrumentation for Java or API based metrics collection for other languages. It also supports distributed tracing frameworks like ZipKin or OpenTracing. It is not provided as a built-in module in OpenShift but it’s really easy to set up on OpenShift and have a Java application being monitored without touching the source code.
 
 Check out these two links:
 
 - https://blog.openshift.com/performance-metrics-apm-spring-boot-microservices-openshift/
 - http://www.hawkular.org/hawkular-apm/
 
 
