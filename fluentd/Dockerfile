FROM fluent/fluentd:edge

# Use root for installing plugins
USER root

# Install Fluentd Elasticsearch plugin
RUN gem install fluent-plugin-elasticsearch --no-document

# Drop back to the default user
USER fluent

# Copy your Fluentd configuration file
COPY fluent.conf /fluentd/etc/fluent.conf