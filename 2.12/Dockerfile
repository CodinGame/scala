FROM openjdk:8

ENV SCALA_VERSION=2.12.0
ENV SCALA_ARCHIVE=http://www.scala-lang.org/files/archive/scala-${SCALA_VERSION}.tgz
ENV SCALA_HOME=/usr/local/share/scala
ENV PATH=${PATH}:${SCALA_HOME}/bin

# Install Scala
RUN mkdir -p "$SCALA_HOME" \
	&& curl -sSL "$SCALA_ARCHIVE" \
	| tar -xzC "$SCALA_HOME" --strip-components=1
