FROM jenkins/jenkins:lts

ENV JAVA_OPTS="-Djenkins.install.runSetupWizard=false"

WORKDIR /var/jenkins_home
COPY --chown=jenkins:jenkins ./jobs ./jobs

COPY plugins.txt /usr/share/jenkins/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/plugins.txt

USER root

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash -

RUN  apt-get install -y nodejs

USER jenkins