# amazon ec2 scalabity 

scalability involves beginning with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out or in. 
as a result, you pay for only the resources you use. 
you don’t have to worry about a lack of computing capacity to meet your customers’ needs.

if you wanted the scaling process to happen automatically, which AWS service would you use? 
The AWS service that provides this functionality for Amazon EC2 instances is Amazon EC2 Auto Scaling.

## amazon ec2 auto scaling

if you’ve tried to access a website that wouldn’t load and frequently timed out, the website might have received more requests than it was able to handle. This situation is similar to waiting in a long line at a coffee shop, when there is only one barista present to take orders from customers.
![scaling](https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1742914800/KxL1Ynp9z42vnMLODBkihQ/tincan/fe470bc5add63f94f005d3da17a6db8131e78b9e/assets/CPE%20Digital%20-%20Amazon%20EC2%20Auto%20Scaling.png)

Amazon EC2 Auto Scaling enables you to automatically add or remove Amazon EC2 instances in response to changing application demand. 
By automatically scaling your instances in and out as needed, you can maintain a greater sense of application availability.
Within Amazon EC2 Auto Scaling, you can use two approaches: dynamic scaling and predictive scaling.

- dinamic scaling responds to changing demand.
- predictive scaling automatically schedules the right number of amazon ec2 instances based on predicted demand

**To scale faster, you can use dynamic scaling and predictive scaling together.**

## Example: Amazon EC2 Auto Scaling

In the cloud, computing power is a programmatic resource, so you can take a more flexible approach to the issue of scaling. 
By adding Amazon EC2 Auto Scaling to an application, you can add new instances to the application when necessary and terminate them when no longer needed.

Suppose that you are preparing to launch an application on Amazon EC2 instances. 
When configuring the size of your Auto Scaling group, you might set the minimum number of Amazon EC2 instances at one. 
This means that at all times, there must be at least one Amazon EC2 instance running.

![auto-scaling-group](https://explore.skillbuilder.aws/files/a/w/aws_prod1_docebosaas_com/1742914800/KxL1Ynp9z42vnMLODBkihQ/tincan/fe470bc5add63f94f005d3da17a6db8131e78b9e/assets/CPE%20Digital%20-%20Auto%20Scaling%20pt%202.png)

When you create an Auto Scaling group, you can set the minimum number of Amazon EC2 instances. The minimum capacity is the number of Amazon EC2 instances that launch immediately after you have created the Auto Scaling group. 
In this example, the Auto Scaling group has a minimum capacity of one Amazon EC2 instance.

Next, you can set the **desired capacity** at two Amazon EC2 instances even though your application needs a minimum of a single Amazon EC2 instance to run.

*obs: If you do not specify the desired number of Amazon EC2 instances in an Auto Scaling group, the desired capacity defaults to your minimum capacity.*

The third configuration that you can set in an Auto Scaling group is the 

**maximum capacity**. 

For example, you might configure the Auto Scaling group to scale out in response to increased demand, but only to a maximum of four Amazon EC2 instances.

Because Amazon EC2 Auto Scaling uses Amazon EC2 instances, you pay for only the instances you use, when you use them. You now have a cost-effective architecture that provides the best customer experience while reducing expenses.
