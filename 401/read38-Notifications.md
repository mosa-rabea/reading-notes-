# SNS

![SNS](https://docs.aws.amazon.com/sns/latest/dg/images/sns-delivery-protocols.png)

* Amazon Simple Notification Service (Amazon SNS) is a managed service that
provides message delivery from publishers to subscribers (also known as producers and consumers).

* Publishers communicate asynchronously with subscribers by sending messages to a topic, 
which is a logical access point and communication channel. 

* Clients can subscribe to the SNS topic and receive published messages using 
 a supported endpoint type, such as Amazon Kinesis Data Firehose, Amazon SQS, 
 AWS Lambda, HTTP, email, mobile push notifications, and mobile text messages (SMS).
 


### Some common cases for private networking and messaging include:

* Isolating development and testing environments
* Sharing personally identifiable information (PII) about your customers
* Hosting a PCI-compliant e-commerce website
* Developing healthcare applications subject to HIPAA
* Implementing a cryptographic algorithm subject to FIPS 140.

### VPC

![VPC](https://www.whizlabs.com/blog/wp-content/uploads/2021/05/AWS-VPC-Components.png)

Amazon Virtual Private Cloud (VPC) is a virtual network that closely resembles 
a traditional network that you’d operate in your own data center.

* Amazon VPC lets you provision a logically isolated section of the AWS Cloud 
where you can launch AWS resources in a virtual network that you define. 
