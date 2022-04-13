![Build Status](http://35.227.235.112/buildStatus/icon?job=dataproc-templates-build%2Fbuild-job)
# Dataproc Templates
Dataproc templates are an effort to solve simple, but large, in-Cloud data tasks, including data import/export/backup/restore and bulk API operations. The technology under the hood which makes these operations possible is the serverless spark functionality based on [Google Cloud's Dataproc](https://cloud.google.com/dataproc/).

Google is providing this collection of pre-implemented Dataproc templates as a reference and to provide easy customization for developers wanting to extend their functionality.

[![Open in Cloud Shell](http://gstatic.com/cloudssh/images/open-btn.svg)](https://console.cloud.google.com/cloudshell/editor)


## Dataproc Templates (Spark)
Please refer to the [Dataproc Templates (Spark) README](java/README.md)  for more information
* [HiveToBigQuery](src/main/java/com/google/cloud/dataproc/templates/hive/README.md)
* [HiveToGCS](src/main/java/com/google/cloud/dataproc/templates/hive/README.md)
* [PubSubToBigQuery](src/main/java/com/google/cloud/dataproc/templates/pubsub/README.md)
* [GCSToBigQuery](src/main/java/com/google/cloud/dataproc/templates/gcs/README.md)
* [GCSToSpanner](src/main/java/com/google/cloud/dataproc/templates/gcs/README.md)
* [SpannerToGCS](src/main/java/com/google/cloud/dataproc/templates/databases/README.md)
* [S3ToBigQuery](src/main/java/com/google/cloud/dataproc/templates/s3/README.md)
* [JDBCToBigQuery](src/main/java/com/google/cloud/dataproc/templates/jdbc/README.md)
* [JDBCToGCS](src/main/java/com/google/cloud/dataproc/templates/jdbc/README.md)
* [WordCount](src/main/java/com/google/cloud/dataproc/templates/word/WordCount.java)
* [GeneralTemplate](src/main/java/com/google/cloud/dataproc/templates/general/README.md)

## Dataproc Templates (PySpark)
Please refer to the [Dataproc Templates (PySpark) README](python/README.md) for more information
* [GCSToBigQuery](python/dataproc_templates/gcs/README.md)
* [BigQueryToGCS](python/dataproc_templates/bigquery/README.md)

## Getting Started

1) Clone this repository

        git clone https://github.com/GoogleCloudPlatform/dataproc-templates.git
2) Obtain authentication credentials

   Create local credentials by running the following command and following the
   oauth2 flow (read more about the command [here](https://cloud.google.com/sdk/gcloud/reference/auth/application-default/login).

        gcloud auth application-default login

   Or manually set the `GOOGLE_APPLICATION_CREDENTIALS` environment variable
   to point to a service account key JSON file path.

   Learn more at [Setting Up Authentication for Server to Server Production Applications](https://developers.google.com/identity/protocols/oauth2/service-account).

*Note:* Application Default Credentials is able to implicitly find the credentials as long as the application is running on Compute Engine, Kubernetes Engine, App Engine, or Cloud Functions.

3) Executing a Template 

    Follow the specific guide, depending on your use case:
   - [Dataproc Templates (Spark) README](java/README.md)
   - [Dataproc Templates (PySpark) README](python/README.md)

## Flow diagram

Below flow diagram shows execution flow for Dataproc Templates:

![Dataproc templates flow diagram](dp-templates.png)

## Contributing
See the contributing [instructions](/CONTRIBUTING.md) to get started contributing.

## License
All solutions within this repository are provided under the [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license. Please see the [LICENSE](/LICENSE) file for more detailed terms and conditions.

## Disclaimer
This repository and its contents are not an official Google Product.

## Contact
Questions, issues, and comments should be directed to
[professional-services-oss@google.com](mailto:professional-services-oss@google.com).

[gcf]: https://cloud.google.com/functions/
[gcf-bg]: https://cloud.google.com/functions/docs/writing/background
[logs-export]: https://cloud.google.com/logging/docs/export/
