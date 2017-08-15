This page/repo contains the slides and demos from the presentation on Software 
Monitoring with Prometheus given at 
[Jax2017](https://jax.de/session/software-monitoring-mit-prometheus/) in Mainz, 
Germany. The presentation can be (re)viewed by clicking here: 
<a href="./prometheus-slides.md" target="_blank" type="text/html"><b>"Software 
Monitoring with Prometheus"</b>, Georg Öttl, Jax2017, Mainz</a>. 
All sources and setups are naturally contained in the git repo backing this page.

```
# Setup environment 
git clone https://github.com/goettl79/software-monitoring-with-prometheus.git
cd software-monitoring-with-prometheus/demo-prom-monitoring-gitblit
ansible-playbook playbook-local-host-setup.yml #adds necessary host entries to your /etc/hosts file
docker-compose up

# Start Browser on Services
google-chrome prometheus.jax.de & \
google-chrome grafana.jax.de/dashboard/db/http-latency-monitoring & \
google-chrome gitblit.jax.de & 

# Start Integration / Performance Tests
mvn install  test -f ../demo-synthetic-monitoring-demo/pom.xml
```

As I'm alwas appreciating feedback, please contact me by twitter. Handle  [@goettl](https://twitter.com/goettl) 

Have Fun and happy DevOps!

