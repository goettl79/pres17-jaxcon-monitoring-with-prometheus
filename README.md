# Software Monitoring with Prometheus

This page contains the slides and demos from the presentation on Software 
Monitoring with Prometheus given at 
[Jax2017](https://jax.de/session/software-monitoring-mit-prometheus/) in Mainz, 
Germany.  As I'm always appreciating feedback please 
<a href="https://twitter.com/intent/tweet?screen_name=goettl&ref_src=twsrc%5Etfw" class="twitter-mention-button" data-show-count="false">tweet to @goettl</a><script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 


## Slides
<iframe src="//www.slideshare.net/slideshow/embed_code/key/f1XmqmirhcMFVu" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/secret/f1XmqmirhcMFVu" title="Softwaremonitoring mit prometheus" target="_blank">Softwaremonitoring mit prometheus</a> </strong> from <strong><a href="https://www.slideshare.net/GeorgOettl" target="_blank">Georg Öttl</a></strong> </div>
<br>
<a href="./prometheus-slides.md.html" target="_blank" type="text/html"><b>Slides Source, Happy DevOps!</b></a> 

## Demo Setup Instructions

```
# Setup environment 
git clone https://github.com/goettl79/pres17-jaxcon-monitoring-with-prometheus.git
cd pres17-jaxcon-monitoring-with-prometheus/demo-prom-monitoring-gitblit
ansible-playbook playbook-local-host-setup.yml #adds necessary host entries to your /etc/hosts file
docker-compose up

# Start Browser on Services
google-chrome prometheus.jax.de & \
google-chrome grafana.jax.de/dashboard/db/http-latency-monitoring & \
google-chrome gitblit.jax.de & 

# Start Integration / Performance Tests
mvn install  test -f ../demo-synthetic-monitoring-demo/pom.xml
```

