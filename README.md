你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# Google Cloud Platform Go Samples

[![Kokoro Build Status][kokoro_badge]][kokoro_link]

This repository holds sample code written in Go that demonstrates the Google
Cloud Platform.

Some samples have accompanying guides on
[cloud.google.com](https://cloud.google.com). See respective README files for
details.

## Contributing changes.

Entirely new samples are not accepted. Bug fixes are welcome, either as pull
requests or as GitHub issues.

See [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.

## Licensing

Code in this repository is licensed under the Apache 2.0. See [LICENSE](LICENSE).

<!---
go list -f '|[{{.Dir}}]({{.Dir}})|{{.Doc}}|' ./... | egrep -v '/(internal|docs/appengine)/' | sed -e "s^$PWD/^^g" >> README.md
--->
## Index

Note: samples under `docs/appengine` are not shown because they mostly do not run, they are just code snippets.

### Getting Started

|Path|Description|
|---|---|
|[getting-started/bookshelf](getting-started/bookshelf)|Package bookshelf contains the bookshelf database and app configuration, shared by the main app module and the worker module.|
|[getting-started/bookshelf/app](getting-started/bookshelf/app)|Sample bookshelf is a fully-featured app demonstrating several Google Cloud APIs, including Datastore, Cloud SQL, Cloud Storage.|
|[getting-started/bookshelf/pubsub_worker](getting-started/bookshelf/pubsub_worker)|Sample pubsub_worker demonstrates the use of the Cloud Pub/Sub API to communicate between two modules.|
|[getting-started/helloworld](getting-started/helloworld)|Sample helloworld is a basic App Engine flexible app.|

### Logging and Monitoring (Stackdriver)

|Path|Description|
|---|---|
|[docs/error-reporting/fluent](docs/error-reporting/fluent)|Sample fluent demonstrates integration of fluent and Cloud Error reporting.|
|[docs/sql/listinstances](docs/sql/listinstances)|Sample listinstances lists the Cloud SQL instances for a given project ID.|
|[docs/storage/listbuckets](docs/storage/listbuckets)|Command listbuckets lists the Google Cloud buckets for a given project ID.|
|[logging/simplelog](logging/simplelog)|Sample simplelog writes some entries, lists them, then deletes the log.|
|[monitoring/custommetric](monitoring/custommetric)|Command custommetric creates a custom metric and writes TimeSeries value to it.|
|[monitoring/listresources](monitoring/listresources)|Command listresources lists the Google Cloud Monitoring v3 Environment against an authenticated user.|

### Compute

|Path|Description|
|---|---|
|[appengine/bigquery](appengine/bigquery)|This App Engine application uses its default service account to list all the BigQuery datasets accessible via the BigQuery REST API.|
|[appengine_flexible/analytics](appengine_flexible/analytics)|Sample analytics demonstrates Google Analytics calls from App Engine flexible environment.|
|[appengine_flexible/cloudsql](appengine_flexible/cloudsql)|Sample cloudsql demonstrates usage of Cloud SQL for MySQL from App Engine flexible environment.|
|[appengine_flexible/cloudsql_postgres](appengine_flexible/cloudsql_postgres)|Sample cloudsql_postgres demonstrates usage of Cloud SQL for PostgreSQL from App Engine flexible environment.|
|[appengine_flexible/datastore](appengine_flexible/datastore)|Sample datastore demonstrates use of the cloud.google.com/go/datastore package from App Engine flexible.|
|[appengine_flexible/endpoints](appengine_flexible/endpoints)|Sample endpoints demonstrates a Cloud Endpoints API.|
|[appengine_flexible/endpoints/client](appengine_flexible/endpoints/client)|Command client performs authenticated requests against an Endpoints API server.|
|[appengine_flexible/helloworld](appengine_flexible/helloworld)|Sample helloworld is a basic App Engine flexible app.|
|[appengine_flexible/mailgun](appengine_flexible/mailgun)|Sample mailgun is a demonstration on sending an e-mail from App Engine flexible environment.|
|[appengine_flexible/mailjet](appengine_flexible/mailjet)|Sample mailjet is a demonstration on sending an e-mail from App Engine flexible environment.|
|[appengine_flexible/memcache](appengine_flexible/memcache)|Sample memcache demonstrates use of a memcached client from App Engine flexible environment.|
|[appengine_flexible/pubsub](appengine_flexible/pubsub)|Sample pubsub demonstrates use of the cloud.google.com/go/pubsub package from App Engine flexible environment.|
|[appengine_flexible/sendgrid](appengine_flexible/sendgrid)|Sample sendgrid is a demonstration on sending an e-mail from App Engine flexible environment.|
|[appengine_flexible/static_files](appengine_flexible/static_files)|Package static demonstrates a static file handler for App Engine flexible environment.|
|[appengine_flexible/storage](appengine_flexible/storage)|Sample storage demonstrates use of the cloud.google.com/go/storage package from App Engine flexible environment.|
|[appengine_flexible/tiny](appengine_flexible/tiny)|Sample tiny demonstrates overall program structure: a main package with a main function that calls appengine.Main.|
|[appengine_flexible/twilio](appengine_flexible/twilio)|Sample twilio demonstrates sending and receiving SMS, receiving calls via Twilio from App Engine flexible environment.|

### Storage

|Path|Description|
|---|---|
|[datastore/tasks](datastore/tasks)|A simple command-line task list manager to demonstrate using the cloud.google.com/go/datastore package.|
|[storage/buckets](storage/buckets)|Sample buckets creates a bucket, lists buckets and deletes a bucket using the Google Storage API.|

### Big Data

|Path|Description|
|---|---|
|[bigquery/syncquery](bigquery/syncquery)|Command syncquery queries a Google BigQuery dataset.|
|[pubsub/subscriptions](pubsub/subscriptions)|Command subscriptions is a tool to manage Google Cloud Pub/Sub subscriptions by using the Pub/Sub API.|
|[pubsub/topics](pubsub/topics)|Command topics is a tool to manage Google Cloud Pub/Sub topics by using the Pub/Sub API.|

### Machine Learning

|Path|Description|
|---|---|
|[language/analyze](language/analyze)|Command analyze performs sentiment, entity, and syntax analysis on a string of text via the Cloud Natural Language API.|
|[speech/caption](speech/caption)|Command caption reads an audio file and outputs the transcript for it.|
|[speech/captionasync](speech/captionasync)|Command captionasync reads an audio file and outputs the transcript for it.|
|[speech/livecaption](speech/livecaption)|Command livecaption pipes the stdin audio data to Google Speech API and outputs the transcript.|
|[speech/wordoffset](speech/wordoffset)|Command wordoffset sends audio data to the Google Speech API and prints word offset information.|
|[vision/detect](vision/detect)|Command detect uses the Vision API's capabilities to detect several types of content (label, text, location, etc) for the given image.|
|[vision/label](vision/label)|Command label uses the Vision API's label detection capabilities to find a label based on an image's content.|

### Privacy

|Path|Description|
|---|---|
|[dlp](dlp)|Samples for the [Data Loss Prevention](https://cloud.google.com/dlp/) API.|

[kokoro_badge]: https://storage.googleapis.com/cloud-devrel-kokoro-resources/go/golang-samples/system_tests-ubuntu.png
[kokoro_link]: https://fusion.corp.google.com/projectanalysis/current/KOKORO/prod%3Acloud-devrel%2Fgo%2Fgolang-samples%2Fsystem_tests
