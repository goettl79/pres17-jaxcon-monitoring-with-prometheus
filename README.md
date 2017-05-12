This page/repo contains the slides and demos from the presentation on Software 
Monitoring with Prometheus given at 
[Jax2017](https://jax.de/session/software-monitoring-mit-prometheus/) in Mainz, 
Germany.  The presentation can be (re)viewed [here](prometheus-slides.md) (german). 
All sources and setups are naturally contained in the git repo backing this page.

```
git clone https://github.com/goettl79/software-monitoring-with-prometheus.git
cd software-monitoring-with-prometheus/demo-prom-monitoring-gitblit
ansible-playbook playbook.yml #adds necessary host entries to your /etc/hosts file
docker-compose up

curl prometheus.jax.de
curl grafana.jax.de
curl gitblit.jax.de

cd demo-synthetic-monitoring-demo
mvn install test
```

As I'm alwas appreciating feedback, please contact me under my by twitter handle 
@goettl

Have Fun and happy DevOps!

