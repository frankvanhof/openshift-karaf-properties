FROM fuse7-karaf-openshift:1.3
EXPOSE 8181 8778
COPY maven /tmp/ca72beeb-64d9-4608-a611-a2b9e916bc95/deployments//
USER root
RUN chown -R jboss:jboss /tmp/ca72beeb-64d9-4608-a611-a2b9e916bc95 && cp -rp /tmp/ca72beeb-64d9-4608-a611-a2b9e916bc95/* / && rm -rf /tmp/ca72beeb-64d9-4608-a611-a2b9e916bc95
USER jboss
CMD /deployments/deploy-and-run.sh
