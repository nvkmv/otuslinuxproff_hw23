# otuslinuxproff_hw23
home work "Prometheus-grafana"

Стенд для демонстрации 

``` vagrant up ```

Поднимется виртуальная машина с адрессом 192.168.1.66 на этот адресс будет настроен Prometheus в файле ``` /dc_prometheus-grafana/prometheus.yml ``` 

На ней будут настроены и запущены два экспортера:
  - node_exporter-1.5.0.linux-amd64
  - предварительно собранный https://github.com/dundee/disk_usage_exporter, для наглядной информации о диске с указанием пути директорий
 
``` docker-compose up -d ``` 

На локальном компьютере запустятся Promehteus port:9090 и Grafana port:3000

  - В Grafana нужно будет импортировать файл дашборда ``` ./nvkm_otus.json ```

  - URLDisk Usage Prometheus Exporter URL: ``` http://prometheus:9090 ```

login/pass: admin/admin

Интерактивный скриншот:

https://snapshots.raintank.io/dashboard/snapshot/VME04ryZmzPE2Pb66U0gcK0eyHbdLz8O

``` screen: ```

![Screenshot_20230209_013120](https://user-images.githubusercontent.com/59445051/217667346-11a8e5c5-2c80-4258-80ea-a8177921db0c.png)


