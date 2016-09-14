FROM jenkins:latest

MAINTAINER jerome.dumas

USER jenkins

ENV JENKINS_OPTS  --prefix=/jenkins 

# installing specific list of plugins. see: https://github.com/jenkinsci/docker#preinstalling-plugins
RUN /usr/local/bin/install-plugins.sh google-login gitlab-plugin gradle sonar android-emulator android-lint jacoco

