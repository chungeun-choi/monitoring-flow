# Monitoring

## Oversview

모니터링을 위한 환경 구축 예시 입니다. 
[[~~Demo dashboard Link~~]](http://demo.cucuridas.info:34322)

### topology

![data_flow.png](data_flow.png)

### **상세 내용**

**사용한 툴** 

collector: `filebeat`, `mysql-exporter`, `node-exporter`, `cadvisor`

transform tools: `Logstash`

OLAP: `Elasticsearch`,`Prometheus`

env build tool: `docker`

**모니터링 대상** 

APP(web-server log): web server에 의해서 생성되는 log 파일

Database(Mysql): DB 엔진의 메트릭 정보를 수집

System(container, system log): system에서 남기는 메트릭 정보, container 메트릭 정보

###
