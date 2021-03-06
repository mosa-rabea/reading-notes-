# Amazon S3
 
* Amazon S3 is object storage built to store and retrieve any amount of data from anywhere. 
It's a simple storage service that offers industry leading durability, availability,
performance, security, and virtually unlimited scalability at very low costs.

* Amazon S3 has a simple web services interface that you can use to store and retrieve any amount of data, at any time, from anywhere on the web.

* A bucket is a container for objects stored in Amazon S3. Every object is contained in a bucket.

* Objects are the fundamental entities stored in Amazon S3. Objects consist of object data and metadata. The data portion is opaque to Amazon S3. The metadata is a set of name-value pairs that describe the object.

![S3a](https://d1.awsstatic.com/re19/Westeros/Diagram_S3_Access_Points.fa88c474dc1073aede962aaf3a6af2d6b02be933.png)


### S3 features

![S3](https://static.javatpoint.com/tutorial/aws/images/advantages-of-aws-s3.jpg)

1. Storage classes: offers a range of storage classes designed for different use cases.
2. Bucket policies: provide centralized access control to buckets and objects based on a variety of conditions.
3. AWS Identity and Access Management: You can use AWS Identity and Access Management (IAM) to manage access to your Amazon S3 resources.
4. Access control lists: control access to each of your buckets and objects using an access control list (ACL).
5. Versioning: use versioning to keep multiple versions of an object in the same bucket.
6. Operations: there are alot of operations like :

+ Create a bucket – Create and name your own bucket in which to store your objects.
+ Write an object – Store data by creating or overwriting an object. When you write an object, you specify a unique key in the namespace of your bucket. This is also a good time to specify any access control you want on the object.
+ Read an object – Read data back. You can download the data via HTTP.
+ Delete an object – Delete some of your data.
+ List keys – List the keys contained in one of your buckets. You can filter the key list based on a prefix.



