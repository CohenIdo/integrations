# AWS Lambda

The AWS Lambda integration allows you to monitor [AWS Lambda](https://aws.amazon.com/lambda/)—a serverless compute service.

Use the AWS Lambda integration to collect metrics related to your [Lambda functions](https://aws.amazon.com/lambda/faqs/#AWS_Lambda_functions). Then visualize that data in Kibana, create alerts to notify you if something goes wrong, and reference metrics when troubleshooting an issue.

For example, you could use this integration to track throttled lambda functions, alert the relevant project manager, and then increase your account's concurrency limit.

## Data streams

The AWS Lambda integration collects one type of data: metrics.

**Metrics** give you insight into the state of AWS Lambda.
Metrics collected by the AWS Lambda integration include the number of times your function code is executed, the amount of time that your function code spends processing an event, the number of invocations that result in a function error, and more. See more details in the [Metrics reference](#metrics-reference).

## Requirements

You need Elasticsearch for storing and searching your data and Kibana for visualizing and managing it.
You can use our hosted Elasticsearch Service on Elastic Cloud, which is recommended, or self-manage the Elastic Stack on your own hardware.

Before using any AWS integration you will need:

* **AWS Credentials** to connect with your AWS account.
* **AWS Permissions** to make sure the user you're using to connect has permission to share the relevant data.

For more details about these requirements, see the **AWS** integration documentation.

## Setup

Use this integration if you only need to collect data from the AWS Lambda service.

If you want to collect data from two or more AWS services, consider using the **AWS** integration.
When you configure the AWS integration, you can collect data from as many AWS services as you'd like.

For step-by-step instructions on how to set up an integration, see the
{{ url "getting-started-observability" "Getting started" }} guide.

## Metrics reference

{{event "lambda"}}

{{fields "lambda"}}