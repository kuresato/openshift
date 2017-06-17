# Grafana and InfulxDB

InfluxDBはDockerHubのOfficialなイメージを使ってデプロイ
> https://hub.docker.com/_/influxdb/

Grafanaは下記URLのDockerfileを使ってOpenShift上でビルドしてデプロイ
> https://github.com/OpenShiftDemos/grafana-openshift

使い方
直接デプロイする場合
```
$ oc process -f https://raw.githubusercontent.com/kuresato/openshift/master/grafana/grafana-template.json SERVICE_NAME=<サービス名> | oc create -f -
```

テンプレートとして登録する場合
```
$ oc create -f https://raw.githubusercontent.com/kuresato/openshift/master/grafana/grafana-template.json
```

