Kafka Container for OpenShift 3
===============================

Version of a popular Kafka Docker image (docker pull spec: confluentinc/cp-kafka)
that will run on OpenShift 3 with the default Security Context Constraint (SCC)
of restricted.

The cp-kafka docker image (at least version 3.3.0) runs fine under the **restricted** SCC already,
so no customization of the image is required at this time.

# Importing Docker image into OpenShift
There is a YAML file in the openshift directory (kafa-imagestream.yml) which will
import the confluentinc/cp-kafka image(s) into the internal registry of an OpenShift
cluster.
