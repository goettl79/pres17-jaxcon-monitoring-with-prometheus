The repo https://github.com/goettl79/software-monitoring-with-prometheus.git contains slides + demos of the presentation given at [Jax2017](https://jax.de/session/software-monitoring-mit-prometheus/) in Mainz, Germany. 

The [presentation](prometheus-slides.md) can be viewed here (german). The demos itself are docker-compose based and can be simply started with a ```docker-compose up```. All sources and setups are naturally contained.

```
git clone https://github.com/goettl79/software-monitoring-with-prometheus.git
cd software-monitoring-with-prometheus/demo-prom-monitoring-gitblit
ansible-playbook playbook.yml #adds necessary host entries to your /etc/hosts file
docker-compose up

curl prometheus.jax.de
```

Have Fun and happy DevOps!

