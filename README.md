# Metabase on Google App Engine

An example of Metabase service on GAE.

## Prerequisites

- Google Cloud SQL
- gcloud


## Setup

Copy and edit `secret.yaml` and replace `<cloud-sql-username>` and `<cloud-sql-password>` with Cloud SQL credentials.

```
$ cp secret.yaml.tmpl secret.yaml
$ vim secret.yaml
```

Edit `Dockerfile` and `app.yaml`.  Replace `<cloud-sql-connection>` with connection information on Cloud SQL.

```
$ vim Dockerfile
$ vim app.yaml
```

Deploy metabase.

```
$ gcloud app deploy
```


## License

MIT License
