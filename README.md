# AWS-CAWS Certified-Solutions-Architect-associate

# Study group
And then I am also building out a study group for the AWS Certified Solutions Architect associate exam. These are just my notes that I have been building since August 2018 and also notes I am sharing with the She Builds (one of the AWS Education Programs) community.

All of this is a work in progress, and I will be adding to this doc hopefully daily. Please feel free to reach out (@julielk) with recommendations or what worked best for you. I love hearing your success stories along with the training that worked for your learning style. Remember, training is personal! But I am trying to create a one source for AWS training to help everyone, no matter your learning style.

# STUDY GROUP covering fundamentals starts here:
HI and welcome the study group for the AWS Certified Solutions Architect certification exam. This study group will not only prepare you to pass the newly released update AWS Certified Solutions Architect, but it will also help you prepare to work as a solutions architect in the real world.

You do not need any previous AWS knowledge, but some will help.

We will start this studygroup with the AWS Fundamentals, and this will be a great refresher or introduction for students that do not have a lot of experience. As we make our way through the content, we will be increasing your skills and confidence because the study material contains both AWS theory, practical demonstrations, and hands-on labs he;ping you to prepare for the certification exam and also get real-world hands-on experience.

# The Exam Blue Print & Slack Community

https://aws.amazon.com/certification/certified-solutions-architect-associate/

https://d1.awsstatic.com/training-and-certification/docs-sa-assoc/AWS-Certified-Solutions-Architect-Associate-Exam-Guide_v1.1_2019_08_27_FINAL.pdf

https://aws.amazon.com/whitepapers/?whitepapers-main.sort-by=item.additionalFields.sortDate&whitepapers-main.sort-order=desc

The exam blueprint adds visibility into what you should see on the certification exam. The AWS CSA SSA exam is usually 65 multiple choice questions and you have 130 minutes to complete the exam. The passing score is 720 and the scores can be from 100-1000 and this certification is good for three years.

If you have never taken an AWS certification exam, usually you will see two correct answers but one of those correct answers is the better choice. You will also see mostly scenario based questions, so you have to be ready to read the scenario questions and pick out key words and phrases to help you choose the most correct answer.

Ok let's get started with our first lesson of AWS fundamentals, cloud computing and AWS.

# What is AWS? Cloud Computing?
Lesson Links:

AWS Website used in this lesson https://www.infrastructure.aws/

Wikipedia website scroll to the bottom https://en.wikipedia.org/wiki/Cloud_computing

What is cloud computing? Well, the AWS website says that cloud computing with AWS provides the most comprehensive cloud platform with over 165 fully featured services from data centers all over the world. So, AWS provides us a way to power our infrastructure while becoming more agile and also lowering our costs. So that is awesome but, what is cloud computing? If you ask around or google what is cloud computing you will find multiple different answers, BUT cloud computing basically means that you have to meet certain criteria.

The first criteria we have to meet for AWS to be considered cloud computing is that AWS has to offer an on-demand self service: and an on-demand self service is the ability to provision compute features or capabilities like servers, databases, networks, storage, and so on…. on-demand, so when that service is needed and also as that service is needed. But we have to be able provision our resources without any human intervention or interaction to make it an on-demand self service. And AWS allows us to do this from the console, the command line, and also using application programming interfaces (APIs). We do not need to request or ask anyone, we can just go in and start building.
The second criteria is that cloud computing needs to have network access to access and provision resources that are needed. AWS allows us to build using the AWS Management Console and the command line using http, https, vpn, ssh, and so on.
The third criteria is that cloud computing needs resource pooling. So what is resource pooling? Well as we will see in this study group, AWS provides pooled resources to serve multiple different AWS customers. So AWS has thousands of servers, databases, and so on that we can on-demand provision and build in our own environment. And these pooled resources are available to me, to you, and to others as well. But another part of this criteria that we have to meet is that we do not know the exact location of these pooled resources and that is okay. For example, when you spin up an EC2 instance you can select the Region, but AWS is allowed to choose any data center in that AWS Region. And we will talk more about aws regions in a few minutes. So AWS procures multiple resources for their aws customers so we are talking about 1000s to make sure they are using economies of scale and you will hear a lot about economies of scale in cost optimization but economies of scale allows AWS with the larger scale of resources, to offer economies at scale to their customers which means that AWS can pass along savings to their customers while also providing customers the resources needed to scale and grow.
The fourth criteria that cloud computing needs is elasticity. Elasticity is the ability to scale with demand. So as your demand increases you can scale up your AWS resources, and then when that demand decreases you can scale your resources back down. AWS provides elasticity.
The fifth and last criteria that AWS must meet to be considered cloud computing is that the resource usage in the AWS accounts can be monitored and billed. So with AWS we are no longer pre-provisioning, procuring your servers, storage, compute, etc. You no longer have to estimate your demands, because with AWS we are not only using services that are monitored for usage and then are billed, but we are also actually scaling those resources to meet your demand instead of being over or under provisioned. And the biggest cost optimization benefit is that we only pay for what we use with AWS cloud computing.

# AWS Global Infrastructure:
https://www.youtube.com/watch?v=gH46jrFfiCc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=2

So how does AWS do this? How do they provide such amazing cloud computing? Well, AWS offers a global infrastructure which is a collection of smaller groupings of infrastructure that is connected by a global high speed network. And this global infrastructure allows us to design systems that are resilient and highly available. AWS offers globally resilient services, regional resiliency services, and also zone resilient services to build a highly available, resilient, fault tolerant system.

So a globally resilient service is a service that operates globally with a single database and that data is then replicated across AWS Regions. A Region can fail, but the service will continue to run. IAM and Route 53 are examples of this.

Region resilient services operate in one Region with one set of that data in that Region and then replicate their data to multiple availability zones inside that Region. So if you lose one AZ in that Region, the service will continue to operate, but if the whole Region fails then so does that service.

AZ resilient are services that are ran in a single AZ, so if that AZ fails, then so does that service. So an exam tip is to know what level of resilience an AWS service has, because it will help you answer exam questions, but also give you a much deeper understanding.

So what is AWS global infrastructure? As we just said, AWS created their global infrastructure as a collection of individual Infrastructures located all over the world. So globally, AWS offers AWS Regions and also AWS Edge Locations.

And AWS is designed to have multiple Regions, multiple AZs, and multiple edge locations around the world. The AWS global infrastructure is made up of AWS Regions around the world - and on top of this global infrastructure, we have high level services.

So we have a level of compute and examples of compute are EC2 and Lambda, then we also have a level of storage like S3 and EFS, and then we also have a level of databases, so RDS Aurora, DDB, etc. And we will cover all of these services in this studt group. So as you can see we have multiple levels of different services on top of the AWS global infrastructure and lets cover the global infrastructure a bit more bc you will see questions on your exam relating to these.

So what is an AWS region, AWS AZ, and Edge location?

Well AWS has over 20 AWS Regions spread across the world. An AWS Region is a geographical area that consists of 2 or more AZs. So there is separation between Regions making each region fault tolerant.

And AWS also has over 50 AZ. An AZ is one or more data centers with redundant power, networking, connectivity, and these centers are housed in separate facilities and sit inside different AWS regions. AWS also have multiple data centers across the world and we can think of an AZ as one or more data centers and incase yo do not know what a data center is, it is a building filled with servers, SANs, switches, load balancers, firewalls, storage etc , and you could have more than one data center in each AZ. So these AZs are isolated compute, storage, network ,etc and you can distribute your infrastructure across multiple AZs in your Region for high availability. So if one AZ fails, then your other AZ should remain operational bc the AZs are isolated from each other but connected with high speed redundant networking and your services can be placed across multiple azs to add resilience and high availability.

And an AWS edge location again is a global service and it is an endpoint for AWS that is used for caching content, and the AWS content delivery network or CDN is CloudFront. And we will cover CloudFront in much more detail throughout the study group, but basically what CloudFront offers is, if a user requests certain information, that information is cached at the edge location, so the next time another user requests that same information that info is already available and delivered to the user much faster then if you had to go all the way back to the database and search for that specific info. Netflix uses edge locations to store content as close to their customers as possible so customers get very low latency when requesting certain movies and shows. The further the data that is being requested is located from customers, the slower the transfer of that data becomes. And AWS has over 150 edge locations around the world.

# EXAM TIP: Make sure you understand the differences between Regions, AZs, and edge locations bc you will most likely see a question on these on your exam.

# Shared Responsibility Model and Well-Architected Framework

Lesson link:https://aws.amazon.com/architecture/well-architected/ and https://aws.amazon.com/architecture/well-architected/

Moving on from AWS as cloud computing, the AWS global infrastructure, we will continue a step farther and discuss the shared responsibility model and also the AWS Well-Architected Framework.

# Share Responsibility Model
What is the shared responsibility model? Well, The Shared Responsibility Model - is how AWS provides clarity around which areas of systems security are theirs, and which are owned by the us, the customer. AWS provides us this shared responsibility model so we are clear which elements of the infrastructure it manages and what elements we are responsible for managing.

At a very high level, AWS is responsible for the security of the cloud, and we are responsible for the security of our data, applications, and so on in the cloud.

In this diagram, the global infrastructure is on the bottom and then different service levels on top of that global infrastructure. Underneath the global infrastructure are the Regions, AZ, and edge locations around the world. AWS manages all of this, the hardware, the security, and so on for the global infrastructure.

And us, as AWS customers, have no control over any of this, so we do not have to worry about this infrastructure.

The next level of the global infra are the levels mentioned earlier: compute, storage, networking, databases, software. And AWS is again responsibility for managing these, the security of these services and systems. So for example, if we choose to provision an EC2 instance from the AWS compute level, AWS manages the Region and the AZ that our EC2 instance will run in.

AWS handles the provisioning and the security, compute, networking storage etc needed for this instance and also handles the software for the EC2 instance.

But now this is where our responsibility comes in. So we are going to be responsible for the operating system and upwards.

So that would be things like client side data encryption integrity, and authentication, server side encryption, and protecting the network traffic. And that includes encrypting your data, using SSL certificates, and so on. We are responsible for all of this as well as the operating system and the network and firewall configurations. We are responsible for our application, and definitely our identity and access management. So we allow people to have certain access to our account and the services in that account. And we will be talking about how to do this in a later section with IAM. We are also responsible for our customer data, securing that data and definitely backups of that data.

# AWS Well-Architected Framework
https://www.youtube.com/watch?v=CeceqWuZ0Cg&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=1

Lets also check out the AWS Well Architected Framework, so what is the AWS Well Architected Framework? Some people skip this part but it is critical to get a solid understanding to help you design more resilient, highly available, cost optimized environments.

The AWS Well Architected Framework is best practices and core strategies for architecting systems in AWS. It helps you design, build and operate reliable, secure, efficient and cost effective systems that will increase your likelihood of success. And AWS has based this on six pillars : operational excellence, security, reliability, performance efficiency, cost optimization, and sustainability.

Get familiar with the design principles:

Stop guessing your capacity - so use autoscaling, have your supply meet your demand
Test systems at production scale
Automate your architecture and this makes experimentation easier
Allow for evolutionary changes and use data to make the needed changes
Improve through gamedays, test runs allow you to see you systems at prod
You may be asking why this is important, why are we discussing cloud computing, the shared responsibility model, and the well architected framework. The reason is that this gives you a good solid basis for understanding AWS, and it will benefit you to take the time to learn and understand these concepts going into your exam.

# AWS Cost Optimization

AWS recently added more cost optimization to the SAA-CO2 exam, so I wanted to add a brief intro to cost optimization and we will also be discussing cost optimization throughout this study group.

Cost Optimization is one of the 6 pillars of the AWS Well-Architected Framework.

Cost Optimization is the ability to run systems that deliver business value at the lowest price point.

AWS offers multiple ways to run a cost optimized env with services: AWS Budgets, AWS Cost and Usage Reports, AWS Cost Explorer, and Reserved Instances and RI reporting. AWS also provides cost effective resources like spot instances, reserved instances and cost effective storage like S3 and S3 Glacier. AWS also allows us to match our supply and demand with Lambda, autoscaling, and so on.

And we can optimize over time using AWS Trusted Advisor, Cost and Usage reports, and we will talk more about these as we complete the study group/

The 5 pillars of Cost Optimization:

The first pillar is rightsizing and right sizing is picking the correct instances for your current resources but also for resources you plan to use. So maybe you are using a larger EC2 instance size when all you need to cover your demand is a small instance size. By right sizing and choosing the correct instance type but also the cheapest instance type that meets performance requirements and can save money.
The second pillar is increasing elasticity and only using resources when those resources are needed and not using resources when they are not needed. This gives us a pay for what we use model. An example of this is that sometimes we can use more smaller instances vs fewer larger instances for our workload and you can reduce your costs. We can use auto scaling to scale up our instances when the demand scales and then scale back down when the demand lessens. And you can schedule instances for periods of demand, usually your production instances will need to be 24/7, but what about your test env or dev env. We can use auto scaling to scale these instances down when they are not being used or during non business hours to save money. AWS provides a tool call the AWS instance scheduler that can create custom start and stop schedules for your instances. And AWS provides this in a CloudFormation template and it is managed by tags, so here is another reason to add a tagging strategy to your env.
The third pillar is to choose the right pricing model and this comes into play after we have right sized our instances and set up auto scaling so we can make sure to meet our demand but also scale back down when that demand is not needed to save money. AWS offers several different pricing models: reserved instances, on-demand instances, and spot instances. And we will cover these too. On demand instances are just as they sound, you can choose to use these when needed, but you can save money by choosing reserved instances, but reserved instances come with a one or three year commitment. But with that commitment you received a lower price. And then we have spot instances which are great if you have a flexible start and end time. And we will cover these too later on. AWS also offers a service called Trusted Advisor which monitors your infra and can recommend how to make our infra more optimized. And then of course use Cost Explorer to monitor your costs.
The fourth pillar is matching our storage to our usage, so reducing your storage can save money because we can match our storage usage to a particular storage class. AWS offers multiple storage classes and we need to make sure we pick the correct one. AWS also offers multiple storage options like S3, EBS, Storage Gateway, EFS, CloudFront, and multiple Data Transfer options and we will cover all of these in much more detail.
And the fifth pillar is to measure and monitor your infrastructure and designs. And this is crucial because your infra will most likely be changing so you need measures in place to monitor and measure your usage and your costs. For this pillar we can monitor our utilization of cpu, ram, storage, etc to identify instances that could be downsized or may need to be increased. AWS provides CloudWatch to track our metrics and CloudWatch also allows us to set alarms so we can immediately take actions. But it is crucial to define your metrics, set target goals, define and enforce your tagging strategy, use cost allocation tags, and make sure you review regularly for any infra changes.
Design principles:

Adopt a consumption model - pay for what you consume
Measure overall efficiency with CW, so make sure to define and track your metrics and goals.
Stop spending money on dc and dc operations
Analyze and attribute expenditures and this simply means track your costs and usages and we can do this with tags, budgets, cost and usage reports, cost explorer and reserved instances like we mentioned earlier
And then use AWS managed services to reduce the overall cost of ownership bc aws can offer lower cost because of economies of scale
Best practices:

The first is to define and enforce Cost Allocation tagging throughout your env. So you can see what resources are costing more. AWS also recommends to use an effective account structure, so this means you need to know what your end goals are and make sure you are designing to meet those goals, along with this AWS recommends to define and use metrics, so not only do you need to know you account structure but you also need to know your goals and what metrics you will be using to track the progress of meeting those goals,

Another huge best practice is to enable your teams to design their architecture based on costs, so let your teams know what the cost is give them access so they can see what they are building and what costs are associated with that cost, once you give a team or person ownership of cost you will find that most are much more cost conscious. And then lastly AWS recommends you create a CCoE, a cloud center of excellence, and this is a team who stays up to date on AWS best practices, new releases,and so on to ensure you are using AWS in the most efficient and cost effective ways. So when we open up our expenditure we make our teams more accountable and more aware to choose more cost effective resources that still match our supply to our demand, but we also make sure we are optimizing our aws account and infra over time.

So as solution architects we have to understand and implement the framework pillars and best practices throughout our infrastructure. You will see a huge change in your org when your operations teams and your finance teams are working towards the same goals.

# High Availability, Fault Tolerance, Disaster Recovery
High Availability (HA), Fault Tolerance (FT), and Disaster Recovery (DR)

High Availability (HA), Fault-Tolerance (FT) and Disaster Recovery (DR) are three essential concepts to understand for every Solutions Architect.

What's more important is understanding the differences between the three - specifically HA and FT.

Let's start with HA, we have already mentioned HA several times, so what is it?

HA is a way to design your systems to have the ability to keep your systems up and running and providing service as often as possible, so it is designed so if a system component fails, then that failure can be replaced or fixed as quickly as possible. So it maximizes the system online time, but HA does not mean it stops failures AND it also does not mean that there will be no down time or outages. HA responds when there is a failure to fix ASAP, so that system can be brought back into service.

HA example: You have an application running on a single server inside AWS, and this server is used by employees to complete their job. If this server goes down, then the employees cannot work because the server is down and it is currently experiencing an outage. So if you design this architecture to be HA, you could quickly spin up a new virtual machine to fail over to. Or you could be running two servers for this application: one server in active and one in standby mode, so if one server goes down, you can failover to the second server to serve the employees. But in this situation the employees may have to log back in so there could be a bit of downtime, which is ok. It is not what you want but with HA some downtime can be expected depending on your design. So the goal of HA is to reduce outages and stay operational, fast and automatic recovery is best. But there is usually downtime even if it is very brief.

Now let's go over FT. What do you think of when you think of FT. It is similar to HA but FT is the actual ability of a system to keep operating in the event of a failure so one or more of the system's components fails, but the system is able to continue on with those faults failing. So a FT design must continue to operate. Let's go back to our earlier scenario, in this case if we are designing for FT then we would have two active servers serving the one application, So if one server goes down then the second server is already active and will continue to serve the employees and there is actually no downtime in this situation. So FT designs operate to minimize failures but also to continue to operate through failure. And these system designs are usually more expensive than HA designs.

DR is a bit different from FT and HA bc FT and HA are all about designing systems to operate through a disaster. DR is all about what we need to plan for and also what we need to do in the event of a disaster.

And having a DR plan is crucial because the worst time to try to recover from a disaster is in the middle of that disaster. DR needs pre-planning and also steps to complete the DR process. So when the disaster occurs you are already set with a plan to recover your systems as quickly as possible. Maybe you have an onsite backup to switch your environment too, or maybe you use AWS as your backup site, and have CloudFormation templates ready to go to provision your env inside AWS after the disaster. And it is essential to have backups of your env stored off site, stored in the cloud but definitely not stored in the same building as your systems. Bc if that building is damaged then so are your backups, so you need a plan to protect your data and store backups elsewhere. And it is best practice to run DR exercise to practice this process, so in a real disaster the process goes smoothly. We must protect systems.

EXAM TIP: Throughout this study group, we will continue discussing these and how different AWS services are great options for one, both, or all, but for the exam make sure you know how to best recover for different scenarios and the best choice for that recovery using different AWS services.

# Elasticity and Scaling
What is scaling?

It is the ability of a system to scale, so increasing or decreasing the load placed upon that system. And systems scale when they need to grow or shrink depending on the load. So when it scales we are adding or removing resources to and from a system. And in AWS, we have two ways to scale: vertical and horizontal.

An example of vertical scaling is if you have a particular size of an EC2 instance and that instance size is not able to keep up with the increase in demand. So the instance may start running very slowly, or in a worst case scenario it may cause the system to crash. So vertical scaling is resizing your EC2 instance to a larger size, if you are using a t2.micro, we may need to resize to a t2.medium or larger. And by resizing your instance we are actually adding more CPU and memory for our system to handle the increase in demand. And if you choose to scale vertically you will encounter a few issues, there is usually a small disruption because the instance when resized will need to be rebooted.

And to tie in Cost Optimization, when you vertically scale to a larger or even larger instance size, you will also see an increase in your cost. And this is one area we can go back to our AWS WAF CO Pillar to make sure we are right sizing our instances in the beginning. But some benefits are that there are usually no application modifications needed and it usually works for all applications.

Now let's talk about horizontal scaling because it was designed to fix some of the issues we have with vertical scaling. So with horizontal scaling instead of increasing the size of our instance, we add more instances of the same size to handle that load. And instead of having one running copy of your application you now have one for each instance that scaled. And we can use a load balancer to help distribute the load across all of our instances.

But we also have to consider certain things with horizontal scaling, one is session, so you do not want to interrupt customer sessions with your applications. When we have a single application running on a single server, then all of our sessions are stored on that server, but what do you think happens to our sessions when we scale to multi servers with copies of our application? Well, sometimes you are shifted between the instances bc horizontal scaling is meant to even out the load so the load balancer sends requests to different servers that have a copy of your application. So AWS recommends to enable sticky sessions so you do not lose your sessions switching between servers. And this works when scaling in or scaling out.

Also, as far as cost optimization, this is usually less expensive because you are using smaller cheaper instance sizes.

Now let's cover Elasticity, what is it? It is an important topic to know and understand for the exam. Elasticity is using automation along with horizontal scaling to match capacity/supply with the demand. You will notice that demand is very rarely linear, it is usually increasing and decreasing, and using elasticity it allows our capacity to increase and decrease and meet that ever changing demand. And AWS provides launch configuration and auto scaling to scale out our systems to match that capacity to that demand, allowing our env to scale out adding additional resources as the demand increases and then when that demand decreases we can scale back in to smaller number of servers or even no servers which optimizes our env for performance efficiency, operational excellence, as well as cost optimization which are all pillars of the AWS Well-Architected Framework.

# EXAM TIP:Vertical scaling is a LARGER size, horizontal scaling is more instances, and elasticity is using automation along with horizontal scaling to match our capacity to our demand.

# Public, Private, Multi, and Hybrid Environments

So in an earlier video we discussed cloud computing and talked about what a cloud environment is, but as you can see we have different types of cloud environments.

Let's start off with a public cloud. What do you think makes a public cloud env? Well, it is simply a cloud env that is available to the public that meets the criteria we discussed in the earlier cloud computing section. And as we know AWS offers a public cloud platform just like Azure and also Google.

And this leads us into the multi-cloud envs, so what do you think a multi-cloud evn looks like? Well, it is still the public cloud env, but you are using more than one public cloud. So maybe you are using AWS and Azure, or AWS and Google, or maybe you are using all three. Which sounds really cool but it is difficult to design and build.

Next we have a private cloud which is pretty cool and private cloud has dedicated services for your env and those services are actually on premises. So these services are dedicated directly to your env. And each cloud vendor has private cloud services, for AWS, it is called AWS OutPosts. But the main difference between having other services on premises and having a private cloud on premises is that the private cloud still has to meet the cloud computing criteria we already discussed, but also be dedicated directly to your business.

And then that leads us into a hybrid cloud which is using the public cloud AND the private cloud together. Some people think a hybrid cloud is using AWS and your on premises data center but it is really not. If you use AWS and also your on premise data center together that is actually a hybrid env. So the difference is there and it is easy to get the two confused. But a hybrid cloud env is a public and private cloud meeting the cloud computing criteria and a hybrid env is using your on premises data center and AWS.

I did not see any exam questions relating to this on my specific beta exam but I have heard others say they had questions on cloud envs so I did want to add this in.

# Public and Private AWS Services
Lesson links: https://docs.aws.amazon.com/vpc/latest/userguide/how-it-works.html

So what do you think AWS means when they label a service as public or private? Well, it is probably not what you are thinking. AWS determines whether a service is private or public by its network. And this is something I really struggled with when I was starting out.

So what is an AWS public service? Well it is a service that can be connected to from anywhere there is an internet connection.

Let's look at a diagram, so inside of AWS we have an AWS public zone and this public zone can communicate openly with the public internet. And AWS public services sit inside this public zone. This is not the public internet ----- remember AWS has its own network and the AWS public zone sits inside AWS but it sits adjacent or sits beside the public internet. And inside of aws, and inside of the AWS public zone is a network that is attached directly to the public internet. So any AWS service that is considered a public service sits and runs from this public zone with the network attached to the open internet. An example of an AWS public service is S3, so when users are connecting to an S3 bucket they are connecting through the public internet.

Now what is an AWS private service? Well it is a private AWS service that lives inside the AWS private zone. And you will see it has no direct connection to the open internet or to the AWS public zone. And inside the aws private zone we can create an isolated env like a VPC or create an EC2 instance and by default it is completely isolated. But we can add permissions for our EC2 instance or for our VPC to access the public zone or the public internet. We simply have to configure the routing or make the instance public and we will be going much deeper into this later. And by default the only services that can access the services inside the private zone are the services inside the private zone. By default there are no permissions for the private zone except your local routes.

# EXAM TIP: In this study group, we will be discussing if AWS services are private or public and you may see some exam questions asking how to give a user or customer access to a specific aws service. And if you understand what makes a service a public aws service or a private aws service and how to design that connectivity then you will be able to confidently answer any questions you may see.

#AWS VPC / AWS Infrastructure (high level overview)
In our Networking and Compute section for this study group, we will cover VPC and compute in deeper details, but I did want to add a high level overview of VPCs to the AWS Fundamentals section.

# EXAM TIP: Now for the certification exam you really need to understand VPCs and know how to build them. You will most likely get 5 to 6 questions on VPCs specifically.

So what is a VPC? Well it is a virtual private cloud, so basically it is your very own virtual data center in the cloud. AWS allows us to provision our own VPC in a logically isolated section of AWS, and we can launch different resources and create our own virtual private network. We have complete control over this virtual networking env, and that even includes choosing our own IP address ranges, creating our own subnet, and configuring access with our route tables and network gateways. And we see in a later section, that we can create a public facing subnet for applications to have access to the internet, but also create private subnets with no internet access to secure our databases and our backend systems. And the VPC offers multiple different layers of security, so we have network access control lists (NACLs) and security groups that we configure to control who and what is allowed to access resources inside our VPC.

https://www.youtube.com/watch?v=jZAvKgqlrjY&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=4

Here is a walk through to create a custom VPC: use this link for the content below on the components of a VPC.

VPCs are created in a Region. The northern Virginia Region, us-east-1, was the first AWS Region and it is the Region that most of the new AWS services are released first, so I usually choose that Region, BUT it is also the Region that goes down the most.

You will notice you have an Internet Gateway (IGW) outside of our VPC and the IGW talks to our router and allows traffic in and out of our VPC to the open internet.

And remember we are going to cover all of these in a later section but I wanted you to have an intro to VPCs in the theory section for this course.

So our IGW then talks to our route tables and remember we configure our route tables with needed permissions for our account. This is part of the shared responsibility model that we are responsible for. Then the requested access is going to hit our NACLs and NACLs act like a firewall and are the first line of defense.

# EXAM TIP: One important tip for the exam is to know all about NACLs and security groups, especially that NACLs are stateless, and what stateless means is that you must add rules for all inbound and also outbound traffic for your VPC. Stateless simply means that the routes for the route tables only see rules one way, so if you add an inbound rule for your VPC, then you must also add an outbound rule to match your inbound rule. So you can add allow rules and also deny rules and another

# EXAM TIP: is that NACLs allow you to block/deny certain IP addresses on your network.

Then we hit our second line of defense which are our security groups and another

# EXAM TIP: Security groups are stateful, and what that means is that any rule that you add to allow inbound traffic will automatically be allowed outbound, so you do not have to add specific outbound rules. Any traffic allowed in, will be allowed back out. And another

# EXAM TIP: is that you cannot deny or block specific IP addresses with security groups, only with NACLs.

We also can create two different subnets, a private and public subnet.

So remember that we can make our ec2 instance public and give them access to the public internet, but we can also make them private with no access to the public internet. So private subnets are great if you do not want traffic accessing your AWS resources, and usually private subnets hold your databases. You can still connect into your private subnet using the EC2 instance in this public subnet. And when you do this the EC2 instance acts as a bastion host or jump box and allows us to access the private EC2 instance or database. So we would follow the access pattern through our gateway, through our NACLs, through the security group. Then from this public EC2 instance we can SSH into our private EC2 instance.

The public subnet is 10.0.1.0/24. And it is a sub network of our VPC CIDR range of 10.0.0.0/16

You choose these IP addresses from 3 different sets of IP addresses that are reserved for private IP addresses that are available for private networks, not for public networks.

10.0.0.0 - 10.255.255.255 which is a /8 prefix which AWS does not allow a /8 subnet, the largest we can have in aws is a /16
172.16.0.0 - 172.31.255.255 and this is a /12 prefix
192.168.0.0 - 192.168.255.255 which is a /16 prefix
Open up cidr.xyz to practice and dive deeper and follow along with the content below.

And we will cover more of CIDRs and subnetting, but if you want to learn more now click the link above. Once you are on the site, if we want to create a subnet for 10.0.0.0/16 we simply enter it in and right away below we can see what our first and last IP address will be and also see the count that shows how many available IP addresses we will have. It also gives us our subnet mask and most people choose this IP address, 10.0.0.0/16, for their VPC because it is the largest subnet we can use inside our VPC.

And then quickly if we change our / to 24 from 16 you will see our info below also changes so now we have 256 IP addresses available. Let's look at a /28 and you will see our count goes all the way down to 16 and this is the smallest subnet that you are allowed to use in your VPC. Anyway this is just an easy and fun tool to help you out. You do not need to really know how to subnet for the exam but it is a great skill to learn early on and honestly I still struggle with subnets. So the earlier you start the better off you will be in your career and for future certifications like the AWS Advanced Networking Specialty exam.

So back to our overview on VPC, we just saw that we can launch subnets inside our VPC and choose the IP address range. We can create an IGW and attach it to our VPC, we can configure our route tables, and we can configure our NACLs and security groups to have security control over our AWS resources inside our VPC. We also have two types of VPCs, we have a default VPC and also a custom VPC.

Your AWS account comes with a default VPC, so you can immediately start building in AWS and you really do not need to know anything. The default vpc comes with subnets, IGW, route tables, security groups, NACLs, and so on already configured for you. EXAM TIP: And for the exam there are differences between the default VPC and custom VPC that you need to know.

All subnets in a default vpc have a route to the internet. Each EC2 instance in the default VPC will have a public and also a private ip address.

VPCs also have some cool features that we will dive deeper into later on. For VPCs to communicate you can add VPC Peering. When you peer VPCs together, the two peered VPCs will behave as if you were using a private network. VPC peering uses the private IP addresses to communicate, you can peer VPCs:

In different regions
With other AWS accounts
Other VPCs in your same account
EXAM TIP: But for the exam, know that VPC peering is not transitive. You must configure each VPC to peer with the other VPC. We do have an option to make our VPCs communicate in a transitive way using AWS Transit Gateway.

So let's quickly do an intro to transitive peering bc it will most likely be on your exam.

Transitive peering with the transit gateway, and we will take a deeper dive into transit gateway, but transit gateway allows transitive peering, so all of the VPCs can communicate with each other.

# EXAM TIPS:

So for the exam, remember that a VPC consists of IGW, route tables, NACLs, security groups, and subnets. You may see a question on the exam about 1 subnet = 1 AZ but you can have multiple AZs in one subnet. And you will most likely have questions regarding security groups being stateful and NACLs being stateless.

# AWS Accounts
https://www.youtube.com/watch?v=rFHnZkx7nqY&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=3

AWS Accounts are not only required to use AWS services, they are also one of the most important tools available to a solutions architect. AWS accounts may seem like a very basic understanding but what accounts are and how they work are crucial bc as a solutions architect you will encounter very simple systems operating in a single AWS account but you will also encounter more complex systems that use tens or even hundreds of aws accounts. So we have to understand AWS accounts.

An AWS account is where you provision your services. It is also where your AWS services log their usage to and also with an AWS account you can log into that environment.

And these AWS services you provision in your account generates a bill and that is billed to you from the payment method you choose when you create your account. It is also important to understand that when you create your AWS account, it is yours. And only yours until you grant access to others. AWS accounts by default do not have permissions until you grant permissions.

We mentioned earlier that AWS isolates usage of the public cloud from other customers of AWS because AWS provides services and some of those services are public services that are shared between different AWS customers. But all AWS services are inside of an AWS account and like we said earlier, all accounts by default do not grant permissions until you specifically grant those permissions.

So when you log into your AWS account you will see that AWS provides authentication. However, when we create our account we are also creating an Account Root User.

And this account root user is given full admin rights to the AWS account. And at this point no one else has permissions on your account, because you must explicitly grant any permissions. You also cannot edit the permissions of your account root users.

Ok, so that is great but how does it work when we create different AWS services in our new AWS account. Well, when you create a new service, like EC2, which we will go into a lot more later on, but for now we should understand that an EC2 instance is a type of a virtual machine. When that EC2 instance is created inside your specific AWS account, right now this EC2 instance would only be accessible by our root user because again we have not explicitly granted any other permissions.

So as you add different AWS resources and services to your account, no one besides the root user account can access those services until we grant permission. And if our account creds are leaked and someone else gets access to our account then only that account is affected. And that is called an isolated blast radius because the security impact for leaked credentials is limited to the one single account.

And as we add services and use them we are charged for the time we use those services. Most AWS services are billed for the time the service is used. For example, if we create an S3 bucket which is a storage service and store pictures in our S3 bucket for a 2 weeks then we are billed for that 2 weeks of storage to our specific aws account.

When we are creating an AWS account, we have to enter credit card information and then that credit card will be used to pay the monthly AWS bill. You can create a billing alarm and stay within the AWS free tier, but you do have to enter a credit card in case you do have usage.

So AWS accounts are the way we access, build, and consume AWS services and our AWS account provides authentication for us to log in, authorization to perform actions in our account, like creating an S3 bucket or an Ec2 instance, and it also tracks our usage and creates a monthly bill.

# Create an AWS Account
Lesson links: https://portal.aws.amazon.com/billing/signup#/start

Plus a blog post with a walk through: https://aws.amazon.com/premiumsupport/knowledge-center/create-and-activate-aws-account/

Let's walk through how to create our AWS account. And it is important to know when you create a new AWS account you have access to AWS Free Tier.

Which is amazing because AWS gives you access for one year and that access is free for a certain amount for the different AWS services, and you can also use certain elements of the different services for free for life of your AWS account. And we will be discussing AWS free tier alot and also AWS cost optimization.

You may notice too as we progress that a lot of people use multiple AWS accounts. You may have a testing account, development account, and a production account, so things are kept separate and nothing interferes with your production account.

To create an AWS account, you are going to need three things:

An email address that is not linked with another AWS account
A phone number where you can receive a phone call or text messages
A valid credit card for our billing method. This credit card will only be used when there are charges in your aws account.
Towards the end, you will have to pick a support plan. You can choose any plan but I usually choose the basic plan which is free. You can see that each plan provides different features that you may need in a real world env AND this is a great EXAM TIP here bc for the AWS certification exam you will need to understand the difference between each of these support plans.

# Securing Your Account Permissions
Lesson Links:

iOS Google Authenticator : https://apps.apple.com/au/app/google-authenticator/id388497605

Android Google Authenticator : https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_CA

1Password : https://1password.com

Authy : https://authy.com/

Let’s secure our new AWS account. Now remember we talked about how our AWS account begins with a single root account user, and remember this user has full permissions to this AWS account and that these permissions cannot be changed.

What we did not talk about is how much of a risk this is, because if our account root user creds are compromised then our whole AWS account is too. So when we logged into our new AWS account remember we added the email address and the password for our root user. And if anyone besides you provides both of these correctly, then they can log into your AWS account as the account root user with full admin creds.

So we want to secure our account permissions so no one, but ourselves can log in as the account root user and take control over our AWS account. And a way we can do this is by adding multi factor authentication to our AWS account. So currently we have an email address and password that is known, so that is considered One Factor. And honestly email addresses are usually pretty easy to figure out. So that would just leave the password. And it is best practice to use MFA and add multi factor authentication to your AWS account and also your users in your AWS account. This adds more security bc MFA not only uses the email address and password that you know, but also adds another factor to enter to log into the AWS account. It uses a one time password also known as OTP, that actually changes on a regular schedule. An MFA can be attached to users inside our AWS account, even our account root user, and once attached in addition to the email address and password, now we also have to provide an OTP, so a one time password that the MFA device generates for us.

So all three will be needed to log into the AWS account. And by using an MFA it makes our aws account more secure because the code changes each time, that code is only valid for a very short time, and that OTP you are given can only be used one time.

Walk through for setting up an MFA on our account root user.

open console

In the AWS mgmt console on the right hand side, let's open the drop down under our account name and select my security creds. And you will see it takes us to the IAM console, the Identity and Access Management console and we will be discussing IAM later on in this section. But you will also see we have security creds and we are being asked if we want to configure our security creds or get started with IAM users.

But we want to configure our security creds, so click, and now we want to open up MFA to activate our MFA. When you see the blue button, click it and now we get to choose the type of MFA device to assign. Choose a virtual MFA device, and click continue. Now we need to download the google authenticator app if you do not already have it, check the links above. Make sure to click show QR code and then you simply scan this QR code with your application. And then the application will begin generating OTP one time passwords for you to enter here below. So you need to enter one code and then wait for the new code to appear and then enter that as well, so you will enter two consecutive OTPs, and then click on assign MFA.

Now we have assigned a virtual MFA to our AWS account and now our root user is more secure.

We will be creating new IAM users, specifically a new admin IIAM user that we will start using instead of our current account root user. That is AWS best practice to use the account root user for your account set up and then only for emergencies. Remember, the root user has full permissions to your aws account. Before we wrap up, another best practice is to enter alternate contacts for AWS to contact you and I always enter my personal info here bc it makes it easier for aws to contact you with any emergencies. There is also the option to add IAM users the ability and permissions to access billing reports, etc. This is a personal choice that you can decide to check the box or not. For my own account I do not want others having this access but again the choice is yours.

# Create a Billing Alarm
https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html

https://www.youtube.com/watch?v=3peNAKB3VxA&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=36

Along with the AWS Free tier, we can create a billing alarm to be notified if we are exceeding a monthly budget. Most of the services you use with AWS are set up so you pay for what you use, or also known as on-demand billing, and services are billed differently in AWS. Some are billed:

per second

per hour

per gig, and so on.

So one important cost optimization tip to know how you are charged for the AWS services you use. And also know that some AWS services offer discounts for a bigger payment up front. But whatever you choose to use, you do pay for that usage each month.

Now AWS offers an amazing option to use the AWS Free tier for a new AWS account for a 12 month period. And the AWS Free Tier is a service that gives you free access to different AWS services, and this is a great tool to use because you can gain free hands-on experience with the different services.

With the AWS Free Tier, you get:

EC2 - 750 hours per month
S3 - 5 gig of standard storage
RDS - 750 free hours
Lambda - 1 million free requests per month, and so on.
So make sure when you are designing your architecture that you understand the free tier usage is different for different services so make sure you have an understanding of what is needed and what is offered for free.

# IAM Intro
Identity and Access Management (IAM) is a core AWS service you will use as a Solutions Architect. IAM is what allows additional identities to be created within an AWS account - identities which can be given restricted levels of access.

IAM identities start with no permissions on an AWS Account, but can be granted permissions (almost) up to those held by the Account Root User.

Right now in your AWS account, you only have our account root user that has full permissions to the AWS accounts. And remember it was created when we created our account and we cannot adjust the permissions for our account root user. But in most cases you will want to grant other people in your organization permissions inside of your AWS account. You will have your different users like your storage team, engineers, sys admins that will need access to the AWS account and also access to the services in your AWS account. It is AWS best practice to practice the principle of least privilege which means only giving access to users in your AWS account to the specific services that they need access too. So users in your account only need permissions to do their job, they do not need any other permissions.

So remember earlier we mentioned reducing our blast radius and another way to do this is too use the principle of least privilege and make sure users in our AWS accounts have the permissions needed but nothing more. So how do we control access to our AWS account and the AWS resources inside the AWS account? Well, this is where IAM comes in and saves the day! Now before we get started with the intro of IAM, I have another EXAM TIP and that is that every AWS account comes with its on copy an IAM which is a database and IAM is a global AWS service that secures any data in the aws iam db across all AWS regions so you can think of IAM as a database service and can do almost anything like your aws account root user.

So let's take a deeper dive into IAM, and IAM allows us to create identities in our AWS account. IAM Users, IAM Groups, and IAM Roles.

IAM users: IAM users represent people and also applications that need access to our AWS account. And you may be thinking really Julie, applications? And yes, sometimes applications need to log into our AWS account to access certain services. And it is important to know for the exam , that IAM identities start with no permissions on an AWS Account, but can be granted permissions needed. IAM Users are one of the identity types available inside AWS. They are the type you pick when you can identify a single individual or 'thing' which will use that identity - a person, an application or a service account. How to create an IAM user in your AWS account?
IAM groups: IAM groups are simply groups of related users, such as your Dev team, your SysAdmins, your storage engineers, and so. And you can even have a group for your finance team to check your usage, and spend of your account. An IAM group is a collection of IAM users and helps to manage IAM users and groups and organize large sets of IAM users. IAM groups have no creds of their own, so groups do not have creds and you cannot log into an IAM group. You may see a question on your exam asking you if you can log into a group and remember that you cannot. You may also see a question asking if an IAM user can be a member of more than one group and the answer is yes. An IAM user can be a member of 10 groups. But there is no limit to how many users can be in a group. If you have an organization of over 5,000 people and you create a group to include everyone in the company, well all 5,000 plus could be added to a single group. But you would have to create that group, and then add the users to that group. There is not a built-in group for all users. Users by defaults have no permissions until we explicitly grant those permissions. There is a soft limit of 300 groups per account but this can be increased with aws by opening a support ticket. EXAM TIP: groups are not true identities like IAM users and IAM roles. They are both considered identities, groups are not. So groups cannot be referenced in an IAM policy because they do not have an Amazon Resource Name (ARN). So IAM policies or even resource policies cannot grant access to an IAM group. A resource policy is a policy on a resource that can reference IAM users and IAM roles using the ARNs. And you may see AS try to trick you on your exam with a question regarding this.
IAM roles: IAM roles are used by AWS services but can also be used to grant external access to your AWS account. For example you would need to grant an EC2 instance inside your AWS account access to CloudWatch, S3, or other services. A role is one type of identity inside our AWS account and the second is IAM users. An IAM user is a single principal. An IAM user is a single thing, a person, an application; it is a single identity needing access permissions in our AWS account. An IAM role is also an identity in AWS. But an IAM role is used by multiple principals, so this could be multiple AWS users, applications, services, inside your AWSaws account, but these could also be users, applications, and so on outside of your AWS account too. So if you are unsure how many principals would need these permissions, then it is probably a good candidate for an IAM role and not an IAM user. And remember that you could use a role if you hit the 5,000 user limits for IAM users. IAM roles are also usually temporary, and roles are assumed. So you assume the permissions/that level of access inside the AWS account and then become that role. And when you stop using those permissions you no longer assume that role, IAM users have long term creds. A role does not represent you like an IAM user does. A role is a level of access or a thing you can use to get the needed permissions. SO with a role you are using permissions for a short period of time; you become that identity for a short period of time.
IAM policies: IAM also has IAM policies. We use IAM policies to allow or deny access to our AWS services, and IAM policies are a bit different because an IAM policy has to be attached to an IAM user, an IAM group, or an IAM role. So you can use AWS Managed Policies or you can create a new policy, and again that policy will simply allow or deny access. On their own policies just sit there, to take action they must be attached to a user, a group, or a role. IAM policies and how aws handles the security of their users and resources. IAM policies are policies that get attached to identities inside of AWS just like we attached the aws managed admin access policy to our admin user. EXAM TIP: identities in AWS are IAM users, IAM groups, and IAM roles. As a solutions architect you will use IAM policies a lot, and you need to understand IAM policies for the certification exam. Two crucial things you need to know for your exam is 1)understand how policies work, how they are designed and architected. 2)Be able to read policies and understand what that policy is allowing or denying. 3) And then I am going to add in a third but it is not required for the exam but it is something you should work towards, and that is to be able to write your own policy, and this third comes with practice and time. More on policies and permissions
So on a high level overview, IAM acts as an ID Provider, or IDP, and it manages identities inside your AWS account, it also authenticates these identities to be allowed to log into your AWS account, and then authorizes those identities to access resources or deny access to resources bases in the policies attached.

Now as far as cost optimization for your AWS account, IAM is free to use, there is no cost, but there are limits to how many users, groups, and so on, you can create.

# EXAM TIP: For the exam, you may see some limitation questions on IAM limits, remember it is a global service, it is resilient. You can only have 5,000 users per account. And an IAM user can be a member of 10 groups.

IAM provides identity federation so AWS allows authentication using AD, google, amazon, and facebook.
It allows us to secure our AWS account using MFA.
IAM identities start with no permissions on an AWS Account, but can be granted permissions needed.
IAM Policies - deeper dive
So what is an IAM Policy? Sometimes you may see them referred to as an IAM Identity policy but they are both the same thing.

It is a set of security statements that grant access or deny access to AWS resources, products, features, and so on.
An IAM policy consists of an IAM Policy Doc that is written in JSON.
There are two types of IAM policies:

# AWS Managed Policy
Inline Policy
Both are the same as the policies we have been discussing but the management is different between the two types.

Inline policy is a policy you create and then apply that policy to individual users. And inline policies are not best practice, but in small envs they can be used. Inline policies are managed individually, so you have to update each inline policy that is attached to users in your account. An advantage of an inline policy is that they are great when you have a special exception to one individual that needs a different set access than anyone else or maybe needs to block access to one user. So remember special or exceptional allows or denies as a reason to use inline policies.
AWS Managed policies are much easier to manage. An AWS managed policy is created with just one version of the needed JSON policy doc, and then you attach the policy to any users that need it. If this policy needs updating you only have to update the one AWS managed policy. If you update an inline policy, then again you must update that policy for each user that uses that policy. Another advantage of AWS managed policies is that you can reuse those policies. And AWS managed policies have two types:
AWS managed policies are managed by AWS.
Customer managed policies are policies we create and manage ourselves.
IAM Roles - deeper dive
IAM roles have two types of policies that can be attached, the trust policy and the permission policy. A trust policycontrols what identity can assume the role. So the trust policy must allow the identity to assume the IAM role. Trust policies can represent IAM users, other IAM roles, and also AWS services, but it can also reference identities in other AWS accounts as well as facebook google, etc.

So if an IAM role gets assumed by something that is allowed to assume it from the trust policy, then AWS will generate temporary security credentials and give those back to the identity assuming the role. And these temporary creds are time limited and only work for short periods of time. When the identity assumes the IAM role with the temp security creds, then it is given access to whatever is allowed inside the PERMISSIONS POLICY.

When you assume a role the temp security creds you receive are generated by an AWS service called Secure Token Service / STS, and you may see an exam question asking what is the operation used to assume a role and that is sts:AssumeRole, you do not need to know the exact specifics or how it works but should remember that name just in case you have an exam question. And if you have a question with sts:AssumeRole you will know that IAM roles are involved. And these temporary creds are time limited and will then expire, but you can renew creds by re-assuming the role. These temp creds can access whatever permissions are in the permission policy

Trust policies can reference IAM users, other IAM roles and also AWS services, but it can also reference identities in other AWS accounts as well as facebook google, etc.

And remember since roles are real identities in AWS just like IAM users and roles can be referenced in resource policies with the ARN for s3 or ec2 and other services.

So lets cover common uses for IAM roles in our AWS account, and the biggest one is for AWS services themselves. So why is this? Well, when we use AWS services, we must explicitly grant those AWS services access and permissions to perform tasks and actions in our accounts. So when we choose to add an AWS service to our account, by default that AWS service has no permissions to act in our account. So the AWS service needs a way to get permissions to do whatever actions you are needing that service to do.

We can create IAM roles that these AWS services can assume with the needed permissions. And the IAM roles will have a trust policy as part of that role like we just saw and that trust policy trusts whatever service we are configuring permissions for. For example, we have an ec2 instance and we need that ec2 instance to log logs into s3. In this case, we would be creating an iAM role for the ec2 instance. That iam role would have the trust policy that trusts the EC2 service. So whenever ec2 needs to send logs to s3, then ec2 can assume this role and use that role to have the permissions needed to put those logs into s3. This IAM role that we create remember also has a permission policy that grants access to services.

Back to our example, our ec2 instance when it needs to put logs into s3, it will use the sts:AssumeRole operation that we talked about earlier and the secure token service to generate the temporary sec creds for our ec2 instance and then ec2 can use the temporary creds to access s3 based on the permissions inside the IAM role's permission policy.

Now if we did not use an IAM role for this access we would need to hard code the security creds on the ec2 instance with the access keys needed. This is not AWS best practice or security best practices. This is a huge security risk because if those access keys are exposed then anyone would have access to do anything. It also causes problems if you ever need to change the access keys. But another EXAM TIP: it is always best practice to choose an IAM role because the service receives temp sec creds to perform the task and it really secures your env vs hardcoding creds. You will most likely see an exam question regarding how to add permissions to aws services and you should make sure to choose iam roles.

IAM roles can also be used when you want to reuse your existing identities from your on premises env and access AWS resources. BC you cannot directly access AWS resources with an external account. However, there is a process that allows you to allow users to use the external identities to access AWS resources.

How it works: you allow an IAM role inside your AWS account to be assumed by an external identity which may be in your on premises Active Directory. It works the same, when the role is assumed by the external identity: temp creds are generated and passed to that external user. And the reason this is important is because AWS accounts only allow 5,000 users per account. If you have more than 5,00o users you would not be allowed to create an IAM user for each of those. Plus that would be a lot of time consuming work plus lots of mgmt of 5000 extra users. But allowing an external identity to assume an IAM role, is called ID Federation and that means using IAM roles with ID federation to give you a smaller number of roles to manage vs over 5,000 iam user accounts. And the external IDs can use these roles to access the needed aws services.

IAM roles are also great for applications that need to access a database in your AWS account because users using a mobile application are most likely going to hundreds of thousands of users, and remember we have the 5,000 user per account limit. But we can use web identity federation and IAM roles for this situation. Most mobile apps allow you to sign in using FB, google, or amazon and the way this works is that our IAM role's trust policy trusts these identities from FB, google, and amazon and again they will then be able to assume that IAM role, they will be given temp sec creds, and then they will be allowed the permissions granted in the permission policy. And by using IAM roles the application has no hard coded creds stored in it which makes the app much more secure and also makes your resources secure as well. And it also uses the customer's existing accounts on amazon, fb, or google, so the user does not need to create a new account. EXAM TIP: You may see a question on your exam asking how to architect solutions for mobile apps and using Web ID Federation along with IAMroles is the way to do that.

# AWS Organizations
AWS Organizations is an AWS product/service that allows larger business and smaller ones to manage AWS accounts with very little management overhead and in a cost effective way. Ok, great but what does this solve, how does it work?

Well without AWS Org it can be difficult to organize and track and manage multiple AWS accounts. Imagine companies that have many AWS accounts. Most large organizations break up their AWS account into multiple AWS accounts: An AWS account for dev and test, one for production, one for security, etc. So in this case, each AWS account has their own IAM users, resources, and so on, but also a separate payment method, because remember each AWSaccount is tracked and billed for the services used to the credit card info you enter when you create the aws account.

So the way it works is from one single AWSaccount, you create an AWS Org, and that account with AWS Org in it becomes the master AWS account of your AWS Org. Then from this master account you can invite other existing AWS accounts into your AWS Org, so they will be sent an invite and those AWS accounts must accept the invite to join your AWS Org. And when they accept the invitation, then those AWS accounts become part of the AWS Org as member AWS accounts. So the way AWS Org is designed is that they can have one master AWS account and then zero or more AWS member accounts. You can also create new AWS accounts from your AWS Org with just a valid email address and if you add accounts this way there is no need for the invitation to be sent, and then also accepted.

The AWS Organization has a root organization similar to our IAM account root user, but it does not have anything special besides acting as a container to hold other AWS master account and or other AWS member accounts.

It also can contain other containers known as Organization Units or Ous, and then these Ous can contain the master and member accounts or other nested organizational units.

So AWS Orgs added simplicity to managing all of your AWS accounts by basically grouping up different accounts to match your business organization AND it also gives you the ability to consolidate all of your AWS accounts into one bill, called consolidated billing. So instead of receiving 5 to 10 individual AWS account bills, AWS Org allows you to consolidate all of your AWS accounts into a single bill. The AWS member accounts pass their billing info to the master account which is the payer account. And this single consolidated bill covers the usage for the master account along with the usage for the aws member accounts.

Another awesome benefit of using AWS Org is that some AWS services get cheaper the more usage that you use, and other aws services are cheaper if you reserve that service and pay in advance for your usage, and with AWS Org, all of these services and usage is pooled for all AWS accounts in the AWS Org, so the all accounts can benefit from the combined cost savings.

You can also use IAM roles to allow access throughout the org to access other AWS accounts in the org. You do not need to create separate IAM users for each AWS member account. And you can use IAM roles, specifically IAM role switch to interact with other accounts

AWS Org has a feature that restricts what member accounts in the org can do and that is called a Service Control Policy SCP. A SCP policy is a JSON policy doc that can be attached to your AWS Org as a whole by attaching the SCP to:

The root container
One or more OUs
One or more AWS accounts directly.
So an SCP inherits down the org structure. If an SCP is attached to the :

AWS Org, affects all accounts in that org.
OU, then they affect all accounts in that OU, and the accounts below that OU.
One or more accounts, then they just affect those accounts.
SCPs are permission boundaries and limit what the accounts can do, including the account root user of that account. So if you have an SCP in your account that prevents usage of an AWS service, then nothing in that account including the root user can use that AWS service. SCPs can limit activity outside of a particular Region, or that allow a certain type of ec2 or rds instance, and so on.

SCPs are used in two main ways:

To block services by default and then allow certain services and this is known as an allow list
Allow by default and block access to certain services known as a deny list.
The default for AWS org is to use deny lists, so allow services by default, and then block access to certain services.

So when you enable SCPs on your AWS Org, AWS will apply a default policy called Full AWS Access for your AWS Org. This policy allows all AWS access, so basically the SCAP has no effect because nothing is restricted and everything is accessible. Again SCPs do not specifically grant access they only control which permissions can be granted, BUT when SCPs are enabled there is an explicit deny, just like IAM policies.

Create an AWS Organization
How to create an AWS Organization

IAM Access Keys
So far in this content, we have only been dealing with AWS access using the console, but we can also access our AWS resources using the CLI and also access resources using apis, sdk, etc.

However, unlike authenticating to the AWS management console, authentication with the CLI does not use our user name, password, and MFA. We authenticate with the CLI using IAM access keys, and like our username and password, access keys are also long term creds,

An IAM user can have two sets of access keys but only one username and one password

So access keys can be created, they can also be deleted, made inactive, and made active.

And an access key is made up of two parts:

Access Key ID which acts like your user name
Secret Access Key which acts like your password
So the Access Key ID is public and the Secret Access Key is private just like a username is public and the password is private. And AWS gives you both of these when these creds are created, but once created, AWS will then discard your Secret Access Key, so it is crucial to copy your Secret Access Key and keep it somewhere within reach but safe. AWS does not store your Secret Access Key, so if you do not copy it and keep it somewhere safe you have no other option than to delete that access key and create a new one.

And that wraps up our AWS Fundamentals section. Next we will dive into a new section covering Network and Compute in AWS.

# Networking and compute

VPC Default Structure
Hi and welcome to a new section on networking and compute and we are starting with Amazon VPCs, let's start off this section and look at the AWS default VPC that AWS provides for all their AWS accounts.

Earlier we talked about the essentials of VPC, so now I want to talk specifically about the default VPC in your AWS Account. So again a VPC is a virtual private network, and it is a service that we use to create private networks in AWS. Our private services will run from this VPC. We can also connect our VPCs from our AWS private network to our on premises for a hybrid environment, or you can connect to other cloud platforms when you are creating a multi cloud env. VPC is a huge part of the certification exam.

When you create a VPC, it is in one region in one AWS account, so this makes a VPC a regional service. And VPCs operate resiliently by operating in multi AZs in a specific AWS Region. By default your VPC is isolated and private until you explicitly grant public access, but there is one exception and you need to know this for your exam and that is the default VPC.

There are two types of VPCs in AWS: the default VPC: you can only have one default vpc per region and also custom VPCs.

Custom VPCs are configured by us as we need them, we are responsible for all of the configurations and by default are isolated and private.
Default VPCs are created by AWS when you create your AWS account and AWS sets up the configuration for us.
Each default comes with one VPC CIDR Range, which is a given range of IP addresses and this VPC CIDR defines the start and end range of the IP address that this default VPC can use. So everything inside your VPC uses this CIDR range, all communications to the VPC will need to use the VPC CIDR and outgoing communications will be from this VPC CIDR. All default vpcs are configured in the same way.

And with your VPC you can divide your network across the azs for resilience, so you can sub divide your VPC into subnets and subnets is short for sub network. Each default VPC is configured to have one subnet located in each AZ of that region. And each subnet in your default VPC uses part of the IP address range of the VPC CIDR. And each subnet's IP address range must be unique to the other subnet’s IP address range and also cannot overlap. So if one of your AZs fails, then that subnet in that failed AZ will also fail, but with the default VPC you have other subnets in other azs that are still operating.

# EXAM TIPS for default VPCs:

You can only have one default VPC per region, it can be deleted and then recreated
You can addIPv6 CIDR but you must enable your VPC for IPv6
The IPv6 CIDR for your subnet range is /64 and the VPC CIDR range is /56
And the local route is used to communicate between subnets inside your VPC
The default VPC CIDR is always the same and designed and configured the same too 172.31.0.0/16 is the default VPC CIDR
/20 for the subnets in each AZ in the region and subnets are assigned public IPv4 address, so they are all public subnets and will be in the aws public zone
And each Default VPC will be provided, an IGW, SG, and NACL

Networking Intro
Lesson Links

https://www.iana.org/numbers

https://en.wikipedia.org/wiki/List_of_assigned_/8_IPv4_address_blocks

Private Addresses RFC1918 https://tools.ietf.org/html/rfc1918

Prefixes : https://www.ripe.net/about-us/press-centre/understanding-ip-addressing

https://www.iana.org/numbers

Before we get too far along in our VPC section, I do want to do a highlevel overview of networking because you may see questions on your exam.

So let's start with the Internet Protocol, known as IP, is how devices communicate in AWS and over the internet. And there are two Internet protocols, IPv4 and IPv6. IF you are interested in a deeper dive into Networking Fundamentals in AWS, check out my YouTube channel.

So IPv4 addresses are represented by dotted decimal notation which consists of four numbers from 0 to 255 separated by a period and the bit between the period is called an octate.

It starts with 0.0.0.0 and ends with 255.255.255.255 giving us over 4.2 billion IP addresses, and this is a large range, but we are running out of IP addresses because these days people have laptops, mobile phones, tablets, etc.

This range was split using classful addressing into smaller ranges

The first range was called Class A and it starts at 0.0.0.0 and ends at 127.255.255.255so that was over 2.1 billion ip address
Then we have Class B and this range starts at 128.0.0.0 and ends at 191.255.255.255 and gives a little over 1 billion ip address
Then we have Class C and this range started at 192.0.0.0 and ends at 223.255.255.255 and gives a little over 2 million ip address
There are also Class D and Class E ip ranges but they are not included in the aws certification exam, so we will focus on Class A,B, and C.
These IP addresses are publicly routed IP addresses, so you can connect to them.

There were also ranges created for private networks to be used in private networks or in AWS

And these IP addresses cannot communicate over the internet they are private. And these IP address were broken down into ranges too:

Class A is 10.0.0.0 - 10.255.255.255 One single Class A
Class B is 172.16.0.0 - 172.31.255.255 16 Class B
Class C is 192.168.0.0 - 192.168.255.255 256 Class C
And our default VPC in AWS is configured in a Class B

So for private IP addresses to communicate with the internet they have to use NAT which is network address translation and we will be covering that a bit later.

This classful process was eventually replaced with CIDR which stands for Classless Inter-Domain Routing. And CIDR removed the limitations of being limited to class A,B, or C size networks.

CIDR addresses are represented by the starting IP address of the network called the network address and the prefix which is a forward slash and a number that represents the size of the network.

So a CIDR looks like this 10.0.0.0/16, so the starting address of the network is 10.0.0.0 and the size of the network is a /16 and for the certification exam you do not need to know much more than a high level of networking, but I will added links above if you are interested you can take a deep dive bc understanding this early on will definitely help especially when you decided to take your AWS Advanced Networking Specialty exam, but for the CSA exam try to remember that the bigger the prefix, the smaller the network, and the smaller the prefix, the larger the network.

So back to our 10.0.0.0/16 will provide a total IP addresses of 65,536

And with CIDR we can split up these IP addresses to create different networks. So we could split it into 2 networks which would be two /17, or 4 networks which would be /18, and so on. This process is called subnetting.

0.0.0.0/0 means all IP addresses, it is the biggest of all networks. So everything
And you may see a slash /32 on your exam. A /32 means 1 IP address. /32 is the smallest network possible
A /8 gives you 16 million ip addresses and is a class A
A /16 gives you 65,536 Ip addresses and is a class B
And a /24 gives you 256 IP addresses and is a class C
IPv6

An IPv6 address is much longer and is represented in hexadecimal rather than the decimal like IPv4 addresses. And is 128 bits long And is called a hextet and because the address is so long we can abbreviate the address by removing redundant zeros.

And the IPv4 networks are also represented by using the start address and a prefix, but with IPv6 each hextet is 16 bits and the prefix number is actually the number of bits that represent the network part of the IPv6 address.

Double colons represent unneeded zeros, so ::/0 means all IPv6 addresses and you may see this on your exam but definitely in AWS.

Subnets
Subnets are what services run from inside our VPC, and they are how we add structure and functionality to our VPCs, and remember that subnets are an AZ resilient feature of AWS.

A subnet is a subnetwork of our VPC CIDR range. And it is created in one AZ, and because it runs in one AZ, if that AZ fails then so will our subnet and the services running inside the subnet. And this is why we need to design our infrastructure for high availability. EXAM TIP: that one subnet is in one AZ, and it can never be in more than the one AZ. But one AZ can have 0 and more subnets. The certification exam may try to trick you on this one, so remember 1 subnet = 1 AZ.

You may have a question on your exam asking what is the IPv6 CIDR subnet range and that is a /64 and the IPv6 cidr range for your VPC is always a/56.

Subnets in your VPC can communicate between each other using the local route.

One thing we did not mention in our intro to networking section above is that some IP addresses inside each VPC are reserved, so we are not able to use those addresses.

And there are 5 ip addresses in each subnet that we cannot use,

The first address that we cannot use is the first address of each network 10.0.0.0
The second address is the Network +1 address and this is the first IP address after our Network Address, so this IP address would be 10.0.0.1 and AWS uses this address for the VPC Router
The third IP address that we cannot uses is called the Network +2 address, so the second ip address after our network address, and AWS uses this ip address for DNS 10.0.0.2
The fourth address that we cannot use and this is the Network +3 address and it is reserved in case it is needed, 10.0.0.3
And the last address we cannot use is the broadcast address which is the last IP in our subnet, 10.?.?.255
So if we should have 16 IP addresses, then we would only actually have 11 IP addresses that we can use, so that is important to know when you are designing smaller VPCs.

Also subnets have a DHCP option set which stands for dynamic host control protocol. This is how computer devices receive their IP addresses automatically, and each VPC comes with one DHCP option set, and can only have one applied at a time, it can be changed BUT for the exam know if you need a new one you must create a new one, you can not edit your DHCP option set.

Routing and Internet Gateway (IGW)
Every VPC has a VPC router that is highly available, and simply moves traffic from somewhere to somewhere else and it runs in all the AZ that your VPC uses. The router has a network interface in each subnet in your VPC and uses the Network+1 address we discussed. You never need to worry about this router, it just works and it's managed by AWS, and routes traffic between subnets in your VPC. We can control this router a bit by creating route tables and associate the route table with the subnet and add rules to allow traffic in and out of your subnets.

Each VPC has a main route table (RT) associated with your subnets, so if you do not explicitly associate your RT with your subnet, then the VPC will use this main RT. A subnet can only have one RT associated with it at a time, but you can use one RT for many different subnets in your VPC.

RTs are created at the VPC level but they are associated with a subnet, which is in one AZ, and only one RT is associated per subnet at a time.

The IGW is a regional resilient service. So it is highly available, and sits on the edge of our VPC and the AWS public zone and the internet. It manages traffic between our VPC, the AWS public zone, and the internet, and the reason we only have one public RT is that the IGW is per VPC, so one IGW works across all AZs.

IF you create a new IGW, you must attach it to the VPC, it is not automatically attached. Then add a route to our RIGHT to allow traffic to and from the IGW. If we add an IGW route to a subnet then it becomes a public subnet because it has access to the aws public zone and the open internet.

The IGW does this by performing a type of NAT called static NAT, and how it works is that the IGW allocates a resource with a public IPv4 IP address. So when the data or packets leave that resource and pass through the IGW, the IGW switches the source IP address from the private IP address to the public IP address and sends the packet on. Then when the packet returns, it switches the destination address from the public IP address back to the private IP address.

Network Access Control Lists (NACLs)
Network Access Control Lists (NACLs) are a type of security filter (like firewalls) which can filter traffic as it enters or leaves a subnet. NACLs are attached to subnets and only filter data as it crosses the subnet boundary. NACLs are stateless and see initiation and response phases of a connection and 1 inbound and 1 outbound stream requiring two roles (one IN one OUT). You will most likely get a few questions on NACLs on your exam.

And by default a default NACL is created for your default VPC associated with all subnets by default.

NACLs are used for traffic entering or leaving a subnet bc NACLS are associated with the subnet not with resources. NACLs only maange traffic that is crossing the subnet boundary. If you have two EC2 instances in your VPC that are communicating, NACLs will have no involvement because the communication between the two instances are not crossing the subnet boundary.

NACLs are stateless and what that means is that if you add a rule for inbound traffic, then you must also add the same rule for outbound traffic. NACLs only see the traffic going one way, so if you allow an inbound rule then you must also allow an outbound rule, so your NACL will explicitly see that traffic that was allowed inbound is also allowed out. NACLs see the traffic as two different streams so you must have two rules, one rule for each stream. IF you do not add your outbound rule, then the traffic will only be allowed in.

NACL rules are processed in order from lowest rule number to the highest rule number, when a rule is matched, an action is taken, and processing stops. An important EXAM TIP is that NACLs can have allow rules or deny rules, and NACLs can explicitly allow or deny specific IP addresses.

All IP communication is actually made up of two parts, the initiation part and also a response part. And a lot of the time, the response part does not use the same port in its response, but instead uses the ephemeral ports. And the ephemeral port range is ports from 1024 - 65535

So with NACLs it is important to remember to add the ephemeral port range.

EXAM TIPS:

NACLs are Stateless
NACLs only affect traffic crossing the subnet border, only applied to the subnet
NACLs can be used to explicitly allow and explicitly deny traffic
NACLs only support IP, Networks, and Protocols, you can not add AWSresources or services
Use NACLs with SGs to add an explicit deny
One subnet is associated with one NACL
NACLs are processed in ordered, so lowest number to highest and ending with the * which is for everything
Security Groups
SGs are another security feature of AWS, only unlike NACLs that are attached to the subnet, SGs are attached to the elastic network interface (ENI) of the AWS resources in the subnet. They also work differently than NACLS. SGs are assigned to the ENI of an AWS resource, so it sits at the boundary, per se, of the instance instead of the subnet.

SGs also have inbound and outbound rules, but SGs are stateful. That means that if traffic is allowed in, then that traffic is automatically allowed back out. SGs see both the inbound and outbound traffic as part of the same stream. One big difference between SGs and NACLs is that SGs recognize AWS resources and you can add rules for these. For example, for an EC2 instance you could add:

The instance ID for that instance to allow traffic from the instance
Rules for other SGs, or add a rule for the SG itself.
SGs also have a hidden explicit deny which means that anything that is not explicitly allowed is denied. BUT for the exam make sure understand SGs cannot explicitly deny a certain IP address, like a NACL can. If you need to explicitly deny, then you need to use NACLs. You will probably see an exam question on this.

EXAM TIPS:

So when would you use NACLs and SGs?

NACLs are used with subnets
NACLS are used for explicit denies
SGs are used for almost everything else and are simpler bc they are stateful there are less rules needed to secure your env
NACLS again are associated with subnet, not with EC2 instances communicating
Custom VPC
Let's cover a few differences between your default VPC and your custom VPC. Your custom VPC is also a regional service like your default VPC. It is an isolated network. And nothing is allowed in or out without explicit configuration. Custom VPC are completely configurable by us. We can create a hybrid network to connect our AWS VPC with our on premises network, and our custom VPC has a choice for default or dedicated tenancy. Default tenancy is resources provisioned inside your VPC that are provisioned on shared hardware with others. Dedicated tenancy is the hardware that is dedicated to you AND dedicated tenancy will be much more expensive. Custom VPCs can use IPv4 CIDR blocks and public IPs and we are given a private IPV4 CIDR block when we provision the VPC. Remember the networking overview, we can choose the largest CIDR range with a /16 - 65,536 IP addresses or the smallest /28 - 16 IP addresses. With your custom VPC you can also have an optional secondary block of IPv4 addresses.

We can also configure our custom VPC with a single assigned IPv6 /56 CIDR block. (we do not get a choice with IPv6 like we can with IPv4). IPv6 are all public IP addresses by default.

Custom VPCs also have fully provisioned DNS, and remember that is the Network +2 IP address. And for the exam you should remember to enableDNSHostnames, then your instances in your VPC will be given public DNS names. You should also choose enableDNSSupport to enable DNS resolution in your VPC. You may see questions relating to either on your exam.

Bastion Hosts
I want to add a high level overview of bastion hosts, also known as jump boxes. We will be covering these under our EC2 instance, cloud compute section. A bastion host is simply an Ec2 instance in a public subnet inside a VPC. And they are a great security feature that can be used to allow incoming management connections into private resources in subnets. It is an inbound mgmt point and you can really tighten up what access is allowed with your RTs.

NAT Gateways
Network Address Translation (NAT) is the process of giving a private resource outgoing access to the internet. TIGW performs a type of NAT called static NAT by allocating a resource with a public IPv4 IP address. When the data or packets leave that resource and pass through the IGW, the IGW switches the source IP address from the private IP address to the public IP address. And then sends the packet on. When the packet returns, it switches the destination address from the public IP address back to the private IP address. So NAT gives a private CIDR range outgoing internet access and to the AWS public zone. And when private resources initiate traffic with a NAT Gateway, they can receive responses back in BUT outside traffic from the internet can not initiate traffic inbound.

AWS provides us two ways to use NAT, using an EC2 instance or by using a NAT Gateway.

Why might a private service need access to the internet? Well the most common reason is for software updates. So software updates are needed, but they also need to stay isolated and private. You can configure your private RT to have a route to the NAT GW, and then configure your public RT to send this traffic from our NAT GWY out. And like the IGW, the NAT GW works in a similar manner;

When the private instance sends data to the NAT GWY, it does so using the RT to the NAT GW from the private RT, the NAT GW then records and stores the source address of the instances sending this packet and also records the destination address that the packet is for. (it can do this for multiple different instances too, in a translation table) Then it adjusts the packets and changes the source address of the instance to be its own source address, the NAT GWY source address, and then uses the route to the IGW to send the packet. The IGW takes the packet from the NAT GW, and then modifies the packet to the NAT GWY public address.

The NAT GWY allows multiple private addresses to masquerade behind it. By using the NAT Source address and then eventually the NAT GWY public IP address that the IGW gives it. So to give private instances access to the internet, you need both the NAT GW and the IGW to complete this and also to configure the routes for the route table.

EXAM TIPS:

NAT GWYs have to sit inside a public subnet bc it needs a public IP address
NAT GWYs also need updated RTs to allow routing
NAT GWYs use elastic IP addresses, an EIP is a special type of IPv4 addresses that are static and do not change.
NATGWs are an AZ resilient service, so for HA you need to add one NAT GWY into each AZ that your VPC uses, update the RTs too for each AZ
NAT is not required for IPv6 bc all IPV6 addresses are publicly routable and the IGW can work directly with IPv6 addresses
NAT GWYs does not work with IPv6
I do want to mention egress only gateways because we just mentioned that NAT GWYs do not work with IPV6. You do not need a NAT GWY for an instance in a private subnet that needs to communicate with the internet for software updates, etc. Because with IPv6 addresses, they are publically accessible and they can communicate with an IGW in a bi-directional manner.

The IPv6 instance can communicate with the public internet and the public internet can communicate with that instance. We can use egress-only gateways instead of NAT GWs for IPv6 instances that we do not want the public internet to be able to access these private instances directly.

With an egress-only gateway, the private instance in a private subnet can communicate with the internet, so it has a route outbound from the instance to the internet. And then that outbound traffic allows the inbound response. BUT with an egress-only gateway, the public internet cannot initiate traffic inbound to this private instance inside the private subnet. So it is an outgoing only version of an IGW for IPv6 instances. Outgoing only that is why it is called egress-only.

VPC Peering
VPC peering is a way to link multiple VPCs together and allows direct communications between two isolated VPCs using their private IP addresses. VPC peers can span AWS accounts and also Regions, and the data shared is encrypted using the AWS global infrastructure.

EXAM TIPS:

Use NACLs and SGs to control access
Why would we use VPC peering?

VPC peering is great for shared services running in a single VPC and you want those shared services to be accessible to other VPCs
To connect your VPC to a vendor or partner system to access an application or in reverse
To give access to your VPC, during a security audit
To meet requirement to split up an application into multiple isolated VPCs to limit the blast radius

https://www.youtube.com/watch?v=6fhwoAwYrug&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=28

VPC Endpoints
VPC endpoints are gateway objects we can create inside our VPC, sort of like IGW and NAT GWYs. They are used to allow instances inside a VPC to connect with AWS public services without the need of a gateway. An IGW or a NAT GWY is not needed. There are two types of endpoints that we need to know the the certification exam:

Gateway Endpoints - A gateway endpoint is used for AWS public services, remember that some AWS services are public services and they sit inside the AWS public zone. Sometimes we want to connect to these public services like S3 or DynamoDB from a private instance or subnet that does not have access to the internet or a NAT GWY set up. Gateway endpoints can be restricted using policies, use routing and need an entry on the RT.

Interface Endpoints - Interface endpoints are used for everything else, and you have to pick the correct endpoint depending on the AWS services. Interface endpoints use security groups, not policies. They also use DNS with a prefix list.

VPC PrivateLink may also appear on your exam. It is an endpoint service that solves the problems of needing to expose an application to other VPCs in other AWS accounts. You could make the application public but then you are using the internet and all is exposed. You could also set up VPC peering, but that is a lot of management overhead and VPC peers must be set up to each VPC. VPC Peering will also expose other applications in the VPCs to the other VPCs. So instead you can configure a PrivateLink. It is the most secure and scalable way to expose a service to 10s or 100s of VPCs and does not require VPC peering, IGW, NAT GWYs, and so on.

If you see any exam questions asking you to expose VPC services to multiple VPCs, the answer is most likely PrivateLink.

https://www.youtube.com/watch?v=iu0-o6hiPpI&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=27

VPN
I want to change the direction of building our custom VPC and talk about connectivity options between our AWS VPC and our on premises networks. AWS has a service, AWS VPN, and it is a service that lets us configure a hardware VPN which is a HA virtual private connection between our VPC and on premises networks. Virtual private networks, VPNs, use the public internet as a transit route for on premises to your VPC. VPNs offer a fully encrypted route from wherever your on premises network is located to your AWS VPC.

So for the exam we need to understand architecture but also when we would want to use VPNs.

And there are three different architectures to know for the exam:

NO HA- A single tunnel between a virtual private gateway/tunnel endpoint and the customer gateway and this does not provide any HA bc if any part fails then we would lose this connection
HA in AWS - Full resilience has two tunnels from the single customer gateway, so we are connecting from a single customer gateway to two tunnel endpoints/virtual private gateways located in different AZs. Dual tunnels do require dynamic routing, so keep that in mind when you are designing your architecture.
Full HA - Here we are creating two customer gateways connecting to two virtual private gateways/tunnel endpoints. Each has two tunnels to the virtual private gateway/tunnel endpoints from the customer gateway. So four tunnels total.
EXAM TIPS:

Remember the three architectures- no HA, HA in AWS, and Full HA
AWS VPN can be set up in minutes, versus Direct Connect that takes months and we will discuss this next
VPNs are fairly cheap, per hour cost and an outgoing data charge that it is a bit higher than Direct Connect, but VPNs are good for lower data transfer requirements
Performance can be limited by your customer gateway router
VPNs offer encryption end to end
VPN performance is variable bc it uses the internet so you can have latency issues
You may get a Route propagation question: local route take priority, then longest prefix, static routes take priority, any routes from Direct Connect over BCP, static VPN routes, any VPN propagated in learned from BGP.
Direct Connect
We just discussed hardware VPN connections. We also have another option to connect our on premises networks and our AWS VPC. And that is Direct Connect (DX). DX is a dedicated physical connection between your on premises network and AWS. Remember a VPN connection is a virtual private connection over the public internet.

DX is a physical piece of fibre running between your on premises network and AWS's network. AWS has a number of direct connect locations that are distributed globally. To get a DX connection, you must have equipment located at one of the DX locations or a deal with a DX partner that already has equipment set up at one of the DX locations.

So DX is a physical or cross connect connection between an AWS router and another router. You can order a DX connection directly from the AWS console.

Once the physical connection is installed and operating we then have to design virtual interfaces (VIFs). And there are two types of VIFs, public VIFs and Private VIFs.

Public VIFS allow you to connect from your on premises network through to any public AWS services, S3, DynamoDB. SQS, SNS, and so on.

Private VIFs allow you to connect, it is a private connection, from on premises to your VPC. These connections are configured much like you configure your VPN connection. Need to create a virtual private gateway, attach it to a VPC, and then create the private VIF and associate it with your virtual private gateway. And then it operates a lot like a VPN at this point.

So if we want to connect to multiple VPCs, we do not have to repeat the above steps, we can create a DX Gateway. It does have to be in the same account but can be in different Regions and the VPCs cannot have overlapping CIDRs. But when you connect to multiple VPCs, the VPCs using the DX gateway does not allow VPC peering with the other VPCs. It only allows connections back and forth between the on premises and individual VPC.





EXAM TIPS:

When you need speed and consistency choose DX because DX has dedicated connections that do not share speed or bandwidth
DX runs over a private cable straight into the AWS network
DX offers low latency bc it does not use the public internet
Bc it is a physical connection, it cannot be configured quickly like the VPN, DX does take at least a week if you already have equipment in the DX location or months if you do not
By default it is not encrypted, BUT VPN is
It is not HA, it is one piece of cable, and equipment in the DX location
You can run a VPN connection along with a DX connection for HA or provision two DX connections for HA
You can always create your VPN first while you are waiting for your DX to become active, and you may see a question on your exam around this
VPC Cost Optimization
I want to wrap up our Network section and talk about cost optimization techniques for your VPC and networking. As we mentioned earlier in AWS fundamentals, it is so important to establish your account structure first. But if you already have an AWS account and you are trying to implement cost optimization, that is awesome!

Remember with your account structure you have defined metrics and goals to track with a business design to achieve the optimal outcome that you or your organization needs to be successful. And make sure you are using cost optimization design principles to design your infrastructure.

Remember to enable Cost Explorer and use the AWS Billing and Cost Management dashboard to track your expenses and usage. Enable tagging and enforce tagging.

EXAM TIPS:

Make sure your EIPs are attached bc you are charged for EIPs not attached in your env
Monitor your data transfer, most data transfer inside a VPC is free and data transferred out is charged.
And remember the fifth pillar of the AWS Well-ArchitectedFramework: measure and monitor your infrastructure. And this is crucial because your infra will most likely be changing, so you need measures in place to monitor and measure your usage and your costs. It is crucial to define your metrics, set target goals, define and enforce your tagging strategy, use cost allocation tags, and make sure you review regularly for any infra changes.
EC2 intro to resilient, elastic, and scalable compute systems
What is EC2 and what does it provide? Well, EC2 is virtualization as a service, it is an infrastructure as a service or IAAS product, and it provides so much value to our AWS accounts.

So, what is virtualization? It is running one or more operating systems (OS) on a piece of physical hardware known as a server. Each OS is separate, along with their applications, and also allows multiple different privileged applications to run on that same hardware using software to make their calls. And this virtualization started off with two different designs and then has kept evolving.

Emulated Virtualization (EV) was the first design of software virtualization. With this design the host OS still ran on the hardware along with a hypervisor that had additional capabilities. And then on top of this was a guest operating system that is known as a virtual machine and then each VM was windows or Linux and had a virtual allocation of resources: CPU, memory, and local disk space. VMs also have other devices mapped to them like network cards, graphic cards, and so on. And to make a long story short, the part of EV to understand is that these guest operating systems believe they are real, not virtualized, and also that they are running on real hardware. BUT this design was very slow because VMs had to talk directly to the hardware.
So Paravirtualization (PV) was created to work on an OS that can be modified. With PV the guest OS is still running in the same design, but instead of calling to the hardware, the OS is modified to have privileged calls become user calls. Those calls are then made to the hypervisor instead of the hardware. So the calls are passed to the hypervisor instead of the hardware, which is quicker and with PV, the OS almost becomes aware of its virtualization which improves the performance.
Virtualization then changed the design, and Hardware Assisted Virtualization was introduced. And in this design the CPU knows it is virtual and contains instructions and additional capabilities to allow the hypervisor to directly configure and control that CPU virtualization. So when privileged calls are made, those calls go to the CPU and then are redirected from the OS to the hypervisor because the OS still believes it is real. Remember the VMs believe they are real, for example, the VMs believe they have a physical network card but what they actually have are logical devices that use a driver that connect back to a physical piece of hardware on the host OS. And this process does consume CPU cycles on the host and can impact the performance.
But there is a last design where the hardware becomes aware of the virtualization, so the network cards and so on. This design is SR-IOV, Single Root IO Virtualization. And the way SR-IOV works is that it allows add-on cards like our example above, a network card, to present itself as mini cards instead of one single network. And as far as the hardware for the VM is concerned, these are fully unique cards and are presented to our guest OS as real cards for its own use, so no translation is needed for the privileged calls. And with EC2, you can use SR-IOV to meet enhanced networking requirements like faster speeds, low latency (even with higher loads), less CPU usage, etc.
EC2 instances are virtual machines, so the OS and also resources: memory, storage, CPU, and so on run on EC2 hosts which are the physical hardware / physical servers that AWS manages. EC2 is the default AWS compute service.

And the EC2 Hosts are either shared hosts or dedicated hosts.

Shared Hosts are the default for EC2 hosts that are shared among different AWS customers, and the customers do not get any ownership of the host hardware. You pay for your individual instances and resources, but it is important to remember that when you use a shared host, your instance is isolated from other AWS customers.
With Dedicated Hosts you are paying for the entire EC2 host, not just the instances you run on that host. You do not share it, you pay for the entire host , no matter how many ec2 instances you spin up.
EC2 instances are an AZ resilient service, because the EC2 hosts sit in an AZ, so if that AZ fails, then the host and the instances running on the host also fail.

EC2 hosts that sit inside an AZ also have local storage, called Instance Store. And the key to understand with Instance Store is that it is temporary. If your EC2 instance moves off the host to another host, then your storage for that instance store is lost. And for networking, you will hear that security groups are attached to your EC2 instance, but this is not necessarily true., The way it works is that when an Ec2 instance is launched into a specific subnet inside your VPC, a primarily elastic network interface (ENI) is provisioned into that subnet and is mapped to the physical hardware of that EC2 host for that AZ. And you can add multiple different ENIs to your ec2 instances.

So let's go back to storage and talk about how an EC2 instance can connect to an elastic block store, EBS. The way this works is that EBS lets you access volumes of persistent storage. Inside your VPC you have a data network set up for your ENIs, but you also have a storage network to connect to your EBS volumes. And EBS is an AZ resilient service, so you can have different EBS volumes running in different subnets for different EC2 instances but you cannot connect an EC2 instance to a EBS volume in a different AZ/subnet.

EXAM TIPS:

Understand the behaviors of Ec2 instances:

Your EC2 is running on a specific host, what happens if you restart your EC2 instance? Well it will stay with that same EC2 host, but if the instance is stopped and then started or if AWS stops the instance for maintenance etc on their end, the instance will be reassigned to another host in the same AZ. So EC2 instances live and remain inside one AZ, but you can migrate your EC2 instance by copying your EC2 instance and then creating a new EC2 instance in a new AZ and a great tool for that is snapshots and AMIs which we will dive deeper into both later. And usually EC2 hosts contain lots of different instances of the same type but different sizes, and we will learn all about instance types and sizes later, but lets quickly mention that you have two types of EC2 instances, burst and steady-state load and again we will cover more depth a bit later on.

EC2 instances
Let's talk about the different types of EC2 instances and a high level overview of which instance type would be the best choice for a particular scenario.

So let's start and look at what we get when we choose and launch an ec2 instance: we get a raw amount of CPU, Memory, Local Storage, and type of storage.

And we need to be aware of the performance for each instance type because with each instance type we will also get storage and network bandwidth, so we need to make sure we have enough bandwidth with the instance type we choose.

We also get resource rations when we choose a particular EC2 instance. And resource ratios are simply the amount of resource you get for each raw amount so for example, an instance that is more suitable to compute would give you more cpu and less memory than an instance more suited for memory which would give you more memory and less compute.

We also get additional features and capabilities with different instance types. Like GPU for graphic processing. Some instances come with GPU and some do not.

So again we come back to your account structure, your goals, your design, and so on. It is crucial to know your design so you know which instance type to choose,

Ec2 instances are group into 5 instance categories: and these categories help you select an instance type based on your particular workload

General Purpose: default steady state workloads, even resource ratios, and should be used as default unless you have specific requirements
Compute Optimize: and these instances are designed for high-performance computing like media processing, ML, gaming, scientific modeling, etc. these resource ration is usually. More CPU than memory and they provide access to high performance CPUs,
Memory Optimized: is great for processing large in memory data sets and database workloads, the resource ration is usually more memory than CPU
Accelerated Computing: is designed for specific requirements like hardware GPU, field programmable gate arrays, FPGAs)
Storage Optimized: is designed for application using data warehousing, analytics workloads, Elasticsearch sequential and random I/Os,
https://aws.amazon.com/ec2/instance-types/

https://ec2instances.info/

And then there are EC2 instance types for each of these instance categories.

Burstable instances: what happens here is that instances have normal CPU loads that are low and you have an allocation of burst credits that allow you to burst up and then return to the normal level. These are usually cheaper and a great option.

When you launch an EC2 instance, you will see the first option to choose is an AMI, an AMI is an Amazon Machine Image. We use AMIs to launch our instances. AMIs are regional so that is important to remember, each individual region has its own regional amis, and amis can only be used in the region it is in. AMIs also control permissions by default that are specific to your account, or you can set the AMI to be public, or add specific AWS accounts on to that AMI. You can also create an AMI from an existing EC2 instance to take the current configuration and make a template to make more instances. And this is great if you have an instance that has a certain OS or certain set of volumes attached, and configured to your exact business requirements, so we can create a template and create an AMI and use this template to create more instances specific to our requirements.

EXAM TIPS:

AMI = one region
AMI baking is the concept of creating an AMI from a configured instance
AMIs cannot be edited, you have to update the conf and then create a new AMI
AMIs can be copied between Regions
Default permissions are only for your AWS account but you can update the permissions
AMIs do contain EBS snapshot so you will be billed for that data stored
EC2 Storage
EC2 has local storage included with the AMI you choose and this storage is called direct attached or local attached storage. These are physical disks that are directly connected to a device, this storage is directly connected to the EC2 host and is called the Instance Store. And this type of storage is really fast bc it is attached to the hardware, but it does have a lot of issues: if the disk fails, if the hardware fail, if the instance moves between two different EC2 hosts, the storage can be lost.

Ee have an alternative type of storage we can use with our EC2 instances and that is Network Attached Storage, and this is where volumes are created and attached to the EC2 instance over the network, and AWS uses Elastic Block Store, EBS, for this. EBS is not as fast as Instance Store, but EBS is highly resilient and is separate from the instance hardware, so issues with the ec2 host will not impact EBS.

You may also hear the term ephemeral storage and this means storage that is temporary you cannot rely on this storage to be persistent. And the instance store is an example of ephemeral storage

And EBS is an example of Persistent Storage, which is permanent storage that lives on even if you delete your EC2 instance.

Now before we go much further I want to talk about the different categories of storage in AWS that we need to know for the exam.

Block storage which we were just talking about, this is EBS, it is a volume that is presented to the OS as a collection of blocks but there is no structure, just a collection of addressable blocks. These blocks can be mounted which means that file systems can be created on top of the block storage, and you can also boot off an EBS volume and this is why most EC2 instances use an EBS volume, block storage, as their boot volume and it is what stores the OS.

EXAM TIP: block storage does not have a structure, and is bootable. And is used if you want to use storage to boot it is block storage, if you want high performance storage inside the OSit will be block storage too.

File Storage has structure, and in AWS this is the Elastic File system (EFS). This is a ready made efile system with a structure. You can create folders and access your files, but you cannot boot from file storage bc you are just given access to a file system over the network but can be used for mounting but not for booting.

EXAM TIP: file storage has a structure, you can create folders, it can be mounted but not bootable. If you want to share a file system across multiple servers it will bd file storage,

Object Storage is a collection of objects and has no structure, it is not mountable or bootable, and can store anything, images, pics, vidoes, files, etc. The key is that object storage is flat and AWS uses S3 for its object storage. If you want access or to store virtually unlimited object data then it will be object storage. Object will be the keyword for object storage and S3.

So for the exam, know the differences between these storage options and their performance.

EBS volumes and snapshots
Let's pick up right where we left off and take a deeper dive into EBS and volumes. Remember EBS provides network storage for our EC2 instances, and we useEBS to create volumes in an AZ and these volumes can be attached to an instance in the same AZ. When we launch EC2 instances, in most cases we are using EBS volumes behind the scenes as our boot volume for that instance. EBS as a service, provides volumes which are allocated block storage and come in different sizes. Volumes are created in an AZ so you have to specify which AZ you want when you create a volume, it is HA and resilient bc the data in a volume replicated within that AZ.

EBS volumes also have different physical storage types to choose from: SSD or HDD and depending on which type you choose you will get varying levels of performance, so you can have more control over your IOPs and throughput.

EBS is billed per month based on a GB gigabyte and sometimes you are billed for a separate IOPs component.

Use EBS if you need HA and reliable persistent storage and if you need to create snapshots.

With EBS we can create 4 different types of volumes:

General Purpose SSD (gp2) and this is the default for most ec2 instances. Gp2 can only be attached to one ec2 instance at a time
Provisioned IOPs SSD (io1) also uses solid state storage, SSD. The biggest difference for provisioned IOPS and gp2, is an increase in your IOPs which is great for high performance low latency workloads that need higher throughputs. Io1 can be attached to multiple instances at the same time. If you have questions on your exam needing High IOPs choose io1.
Throughput Optimized HDD (st1) uses magnetic drives HDD, the t in st1 stands for throughput; you cannot boot on either HDD type of volume. The big difference between these two is the type of HDD types is the data needing storage, st1 is designed for frequently accessed throughput intensive workloads, like data warehousing.
Cold HDD (sc1) uses magnetic drives HDD based, the c in sc1 stands for cold so if you have any questions regarding needing cold storage, choose sc1. This type is designed for data that is less frequently accessed and cannot be used for a boot volume.
You can pick your volume type based on your performance needed.

So if you need maximum IOPs pick GP2 or io1 great for databases
Or if you need higher throughput pick st1 or sc1 great for log storage
Lets also cover EBS snapshots bc they are a really useful feature of EBS. Snapshots are a backup of our EBS volumes. Snapshots are incremental volume copies that are saved in an S3 bucket. The first snapshot is a full copy of your data on that volume, and then the next snapshots are only incremental copies so only data that has changed. And this can protect your data against any AZ issues because the data stored in s3 becomes Region resilient. So when we create EBS volumes, we can create a new volume or create a volume from a snapshot, and you can use snapshots to copy data to multiple AZ and also Regions.

As a SA, you have to be aware of snapshot performance for the real world and also your exam.

When you create a new EBS volume, there is no need to do any initialization, the full performance is immediately available, but if you restore a EBS volume from a snapshot it does take time to initialize, and if you attempt to read data that is not restored yet, it is very slow.

But you can force a read of all data immediately when you are completing a restore especially in production. Fast snapshot restore, FSR, makes the instance restore immediate. And you get 50 snaps per Region and FSR is an added cost.

And let's also cover EBS encryption: By default EBS volumes have no encryption, but EBS encryption does provide at rest encryption.

When you create an EBS volume initially it is not encrypted but you can choose to enable encryption, and when you do, EBS uses KMS and the customer master key. And we will cover AWS Key mgmt service in a later section. But when an encrypted volume is created, then KMS uses the CMK to create a data encryption key to encrypt the volume and can only be decrypted using KMS. If you make a snapshot of an EBS encrypted volume the same data encryption key is used for the snapshot, so the snapshot is encrypted and any new volumes made from these encrypted snapshots are also encrypted and share this key. But if you create a new EBS volume from scratch with encryption you will get a new data encryption key.

EXAM TIPS:

EBS volumes are created in AZ,
EBS is HA and resilient bc its data is replicated inside the AZ
With EBS volumes you can also create a snapshot to offer more HA
Usually with EBS you can only have one EBS volume attached to one EC2 instance at a time, but we now also have a multi attach option with Provisioned IOPs but you probably will not see that on your exam yet.
EBS has gigabyte per month cost
AWS accounts can be configured to encrypt EBS volumes by default
Each volume uses a unique data encryption key and snapshots and future volumes from your snapshot use the same dek
Once an EBS volume is encrypted you cannot select to un encrypted the volume
EC2 Instance Store
Let’s cover the second storage option for our EC2 instances, Instance Store.

EC2 has local storage included with the Amazon Machine Image (AMI) you choose, and this storage is called direct attached or local attached storage.

These are physical disks that are directly connected to a device. This storage is directly connected to the EC2 host and is called the Instance Store.  And this type of storage is really fast because it is attached to the hardware. But it does have a lot of issues:

If the disk fails,
If the hardware fails, or
If the instance moves between two different EC2 hosts, then
the storage can be lost.

So for the exam we need to be aware of the benefits and issues with instance store as well as when you would choose instance store in different scenarios.

Instance store is another block storage device, but ulike EBS, instance store is physically connected to one EC2 host. So that location for instance store actually gives it the highest storage performance because it is local to the EC2 host, and must be attached when the instance is created. You cannot attach an instance store volume after your launch an instance. And instance store volumes are included in the instance cost.

Remember that instance store is ephemeral storage, so they are temp storage, and as a SA you must consider this temp storage.

If an instance with instance store moves to a new EC2 host, that storage will be lost. If an instance was stopped and started, it will also lose the instance store volume. If you change the type of your EC2 instance you will also lose that storage. If you have a hardware failure, you will lose that data. And the number of instance store volumes and size you get with your instance is based on the type of instance you choose.

But the big benefit of instance store is that it gives you higher performance, because again, that instance store is local to the EC2 host, and it is so much more faster BUT it is only temp storage.

EXAM TIPS:

Instance store volumes are local to an EC2 host
You can only add instance store volumes to an instance at launch time
Data is lost if that instance is moved to another host, resized, restarted, or has hardware failures, and so on
Gives the highest data performance in AWS but comes with the risks of losing that temp data
Instance store volumes are included in the cost of the instance
So let’s cover scenarios when you would want to choose EBS volumes over Instance Store volumes and vice versa.

When to use EBS:

Remember EBS is HA and is reliable persistent storage. So if you need reliable and available data then choose EBS.
Also consider that EBS is separate from EC2, and can be attached to one instance, and then detached and attached to another instance. So if you need to have persistent storage that you can move to another instance choose EBS, and remember we can now multi attach volumes to more than one instance at a time, so EBS would be a choice for this scenario too.
With EBS we can create snapshots and create backups for our data, this cannot be done with instance store volumes.
Remember for the exam the cap for EBS volumes is under 80,000 IOPS anything more we need to choose instance store.
When to use instance store:

Instance store volumes are a great value and are included in the instance price, and the larger the instance size the more instance volumes you usually get.
BUT if you need high fast performance greater than 80,000 IOPs or more than 2,375 megabytes per second choose instance store.
Also great if you need temp storage, especially since it is included with your instance price.
Also great for stateless services that do not store any account or session info.
Elastic File System (EFS)
I want to cover Elastic File System (EFS) in our EC2 section we may dive deeper into EFS in the storage section.

EFS is really useful with most AWS infrastructures because it provides network based file systems that can be mounted within Linux EC2 instances. It can then be used by multiple EC2 instances at the same time. So it allows us to store data outside of the EC2 instance while providing scaling and self healing properties.

AWS EFS is the AWS version of NFS, network file system, version 4. And with EFS you create file systems and then those file systems can be mounted on EC2 (Linux) instances. EFS systems can be mounted on many EC2 instances and that data in that file system can be shared within the file system with all of the EC2 instances.

EFS is separate like EBS, but lives inside a VPC, and can be accessed via hybrid methods like VPN or DX which are hybrid network systems which we will cover in a later section.

EFS runs inside our VPC and we create file systems inside EFS. EFS is accessible because there are tagerts mounted inside each subnet in multiple AZs that adds HA, and your instance uses the mount targets to connect to EFS.

EXAM TIPS:

EFS is only for Linux instances
Two performance modes, General Purpose (GP) and Max I/O
GP is the default and is great for latency sensitive use cases: web servers, directories, and so on.
Max I/O can scale to higher levels of throughput with added latency, so there is a trade off, great for media processing
And for throughput we have two different throughput modes:

Bursting mode works like EBS GP2 volumes
Provisioned you can specify throughput separate from size and is more like provisioned IO1
EFS also has two storage classes:

Standard - default and used for data frequently accessed files
Infrequent Access - less expensive and for data that is not often needed
And you can also use lifecycle policies to move data between the two different storage classes

EC2 user data and bootstrap scripts
In an earlier lesson we talked about Amazon Machine Images (AMIs), metadata and bootstrap scripts, so I want to take a deeper dive and cover at a high level overview of EC2 metadata and bootstrap scripts and what we need to know for our exam.

Bootstrapping on an EC2 instance is the process of configuring an EC2 instance to perform automated installation and configuration steps before that instance is brought into an in-service state. And with an EC2 instance we accomplish this by passing a script via the user data part of the launch configuration. And this process will help an instance come into service when it is in a preconfigured state with configuration or software installed.

Bootstrapping is just a process that helps to build automation and to bring the instance in-service with a pre-configured state. This process performs software installation.

169.254.169.254/latest/user-data

169.254.169.254/latest/meta-data

These are internal IPs for AWS.  You can retrieve the IAM role from the metadata, but not the IAM policy along with the AMI ID, the instance ID, the host name, instance type and so on for our EC2 instance.

And for the exam you need to know the difference between metadata and user data:

Metadata is the info about the EC2 instance
User data is the launch script of the EC2 instance
And the user data is a piece of information that we can pass into an EC2 instance and it is executed by the instance's OS only once at launch time. So it only applies to initial launch.

Previously, we used an AMI with an eBS volume, but now the EC2 service provides user data to this instance, and will check the metadata IP for any user data.

EXAM TIPS:

User data is a simple block of data

User data is not secure, do not pass in creds in your user data

User data is limited in size, but you can pass in scripts to download that need data

User data can be modified when an instance is stopped

But only executed during initial launch

For the exam you may see a question asking how quickly can you bring an instance to in-service state, and for AWS AMIs is usually only minutes, but sometimes we need time to install apps, etc. so we need the time to be extended before an instance is in an in-service state.

And bootstrapping helps us install needed software before an instance progresses to the in service state much quicker

We can also bake this software into an AMI. AMI baking allows you to add the needed software to be added to the AMI before the instance is launched. So all the software is included in the AMI. And you can use both to provide optimal progression and with bootstrapping and the baked AMI you can get more flexibility with the configuration.

EC2 Bootstrapping is the process of configuring an EC2 instance to perform automated install along with configuration steps post launch before an instance is brought into service.

With EC2 this is accomplished by passing a script via the User Data part of the Meta-data service which is then executed by the EC2 Instance OS.

ENIs, IP addresses, and DNS
In this lesson I want to tie in some of the networking we mentioned earlier to get a better understanding of how your can interact with EC2 instances and connect to EC2 instances.

Architecture of an EC2 instance:

Each EC2 instance starts out with one elastic network interface (ENI), the primary ENI. You can also attach one or more secondary ENIs that can be in separate subnets but in the same AZ.

The ENIs are separate from the EC2 instance, not attached to the instance themselves. The primary ENI has the actual IP address for the EC2 instance, even though it appears that those IP addresses are attached to the instance, they are actually attached to the primary ENI for that instance.  When you launch an instance with security groups, the security groups are also attached to the primary ENIi not the instance itself.

The primary ENI has a Mac address and primary IPv4 private IP address. You can have zero or more secondary IP addresses for private and public IP addresses, and you can have 1 elastic IP Address (EIP) per private IP address. You can also have one or more IPv6 addresses, and you can have security groups.

Per ENI, you can enable or disable the source destination check, so if traffic does not match the address the traffic will be discarded and for NAT gateways this needs to be disabled.

You cannot detach the primary ENI, but you can detach other secondary ENIs and move them to other instances.

EC2 instances will also receive DNS addresses that can communicate with the private IP addresses inside your VPC.

EIPs: when we allocate an EIP we can associate the EIP with our primary ENI or our secondary ENI.  If we assign an EIP, then the instance will lose its public IPv4 address, if you remove the EIP then you get reassigned a new public IPv4 address.

EXAM TIPS:

SGs are attached to the ENI, not SGs
You can set up different SGs for multiple ENIs to have more secure connections
If you stop your instance, a new IPv4 address will be given to that instance. EIPs can solve this problem
Public DNS will resolve to your primary IP address inside your VPC, but the public DNS will resolve to the public IP from everywhere else.
EC2 Auto Scaling
Auto scaling groups (ASGs) are how we configure EC2 to scale automatically based on different criteria.  ASG uses launch templates or launch configurations.

A launch configuration:

ASG provides autoscaling for EC2 and can be used to implement a self-healing architecture, and they use the launch configuration to know what to provision.

ASG has three important values to remember:  minimum size, maximum size, and desired capacity. And an ASG provisions and terminates based on the number of instances they have currently and what the desired capacity is set too.

How it works:

If the desired capacity is more than the instances we have provisioned, then the ASG will launch new instances to match that desired capacity.
If the desired capacity is less than what is provisioned, then the asg will terminate instances to bring the actual number to match the desired capacity.
And we can use scaling policies based on metrics like CPU utilization.

If you have our launch configuration (min, max, and desired capacity) set to:

Minimum size: 1 instances

Desired capacity: 2 instances

Maximum size: 4 instances

Your launch configuration and auto scaling group will look and see you have:

1 instance for your min size, you will always have one running instance.
2 instances for your desired capacity, your ASG will take this launch configuration with a desired capacity of two instances and launch a new instance to match the 2 instances for your desired capacity.
4 instances for your max size, you could potentially have up to 4 running instances at a time depending on the metrics we assign.
So this can be done manually or we can add scaling policies to do this automatically. A scaling policy is rules that we define that adjust our values with our ASG. We also have scheduled scaling policies that are based on time-based adjustments. Dynamic scaling that are rules that react to a metric, and under dynamic scaling we have three sub policies:

Simple scaling, so it is a rule on a metric, so let's say our CPU utilization, memory, or disk I/O is greater than 50%, then add 1 instance. If the metric is lower than 50% remove one instance. This allows scaling in and out based on the metrics.
Stepped scaling defines more detailed rules. So add 1 instance if the metric tracks over 50% or add 3 if the metric is over 90%.
Target tracking is configured to define an ideal metric. Maybe you want your CPU utilization to stay around 40%. The point here is to maintain that level, and the ASG will adjust the size-in and out to maintain the value.
ASGs also have cool down periods which control how long to wait at the end of a scaling action before performing another action. You can use cool down periods to make sure scaling actions do not occur until a certain time has expired.

ASGs can also be configured to replace failed instances. The way it works is that it will see an instance has failed. The ASG will terminate the instance, and then launch a new instance to replace the failed instance. This self-healing feature is what we talked about earlier, in this situation the launch configuration would be a min of 1, max of 1, and desired capacity of 1.

ASGs can be used with load balancers. Load balancers use listeners that are configured and are pointed towards a group of EC2 instances in a target group. A target group is just a set of instances; you can link your ASG with this target group. And this is usually based on the load of the system to determine the scaling policy.

ASGs can use the load balancers for their health checks rather than the EC2 instances health checks.  Application load balancers have health checks that are a lot more defined and application-aware than the simple status checks of EC2.

EXAM TIPS:

ASGs are free at no costs, just the resources that the ASG creates.

ASGs use cool down periods and avoid rapid scaling

Use smaller instances bc it offers more granularity and has a cost savings over larger instances

ASGs and ALBs offer more elasticity because they are not connecting to the servers but to the load balancer, so they are abstracted from the instances and can use that capacity more smoothly.

ASGs define when and where to launch and the launch configuration defines what you want to launch

Launch configurations define what is launched:  what type of instance, what networking, what SGs, what AMIs, and so on.

ASG defines when and where to launch the instances, what subnet, what vpc, and so on.

Storage, Databases, and Migration
Storage intro
Earlier we covered requirements to consider when choosing a storage solution, but we also have to add into our considerations:

· Durability

· Availability

· Security

· Regulatory and governance requirements and

· Functional requirements

AWS storage solutions can meet different technical and price requirements. From a cost-optimization perspective, the lowest compute-related cost storage option is locally attached, ephemeral storage. This is storage included in the run rate for EC2 instances. The local processing nature of ephemeral storage isn’t for long- term, persistent data storage.

For more persistent storage, Amazon Elastic Block Store (Amazon EBS) enables EC2 instances to write to block-level devices that can be migrated to different instances. It also provides snapshot functionality to back up and migrate these volumes.

There are two storage types available for EC2 instances: non-persistent or ephemeral storage, which is appropriate for log files and non-critical data, and persistent storage for applications and workloads that require persistency.

Each option has pros and cons in terms of performance and costs. Ephemeral storage is included in the EC2 instance hourly rate. Amazon EBS comes at additional cost. You should consider these pros and cons per workload during your initial assessment, and then again after the workload has been running for a time. That way, you can see if you’re using the resources you’ve allocated and

make adjustments, if necessary. For example, among the Amazon EBS volume types, you could switch from Provisioned IOPS to GP2 instances if you find that your workload is more efficiently run on a “bursting” level of IOPS. AWS makes volume information available to customers through Trusted Advisor, which will highlight unattached Amazon EBS volumes and other important deployment information. In this case, with a proper archive strategy, deleting unattached Amazon EBS volumes will minimize storage costs.

Amazon S3
S3 is accessible from anywhere in the world with an internet connection and providing 99.999999999% durability. S3 has no limits on the amount of storage that can be used and provides mechanisms for customers to delete or archive (to Amazon Glacier) data no longer needed in quick-access storage. Using Amazon S3 lifecycle policies will enable you to migrate data from Amazon S3 to Amazon Glacier or delete it entirely. Amazon S3 also provides customers with storage classes8 with different levels of durability, availability, and pricing. These other classes can be useful when your storage mechanism does not require 99.999999999% durability.

https://www.youtube.com/watch?v=vFfY_-TL-pc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=6

Amazon Glacier
You can use Amazon Glacier to address your archiving requirements and improve your cost optimization. Amazon Glacier is, by design, cold storage. It should be used for data you need to retain, but do not need to frequently access. Although S3-to-Amazon Glacier migrations can be seamless, many small, frequent retrievals from Amazon Glacier will cause you to incur higher costs. For this reason, you should carefully consider a retrieval process.

https://d0.awsstatic.com/whitepapers/Cost_Optimization_with_AWS.pdf

Storage Gateway
Storage gwy is a service that allows us to connect your on premises data center and storage to AWS storage service. It allows us to migrate part or all of your storage platform to AWS or it supports extending your storage platform to AWS.

And we have three types of storage gwy:

File gateway: stores files as objects in S3 but has a local cache for your most recently accessed data onsite. Storage gwy is virtual appliance that you run on premises as a virtualization platform, so you can run it on VMware, esxi, ec2, and so on. You download and configure on your on premises location to talk to aWS over the internet. File gateway is a great option for Windows and is accessible using SMB and when you upload data with your storage gwy, that data is stored in S3.

Volume gateway: is configured the same way as file gateway. You configure and download the virtual machine image. However, when you access volume gateway, you are not accessing file shares, but volumes and these volumes are accessed over the protocol I-SCUZI which is generally used with SAN products, so it is network attached storage, and volume gwy works great with servers. You can also take snapshots from the volumes and create EBS volumes.

These are iscuzi presented volumes, and you cannot access the files indivudally without mounting the entire volume.

And you have two options for volume gateway:

Gateway stored volumes: which helps to store all your data on a volume gwy applicance itself and then snapshots are taken into aws stored on s3. This is used when you want your data on premises but snapshots backups in s3.

Gateway cache volume: which stores primary copy of your data in AWS and then downloads and caches frequently accessed data on the volume gateway itself.

Virtual Tape Library gateway: allows us to present a virtual tape library over ISCSI to any compatible backup software. This has a high admin overhead and is also costly, and should be stored off site. Allows us to present a virtual tape drive and it is stored in S3. Can be used to migrate your data into AWS over a period of time.

EXAM TIP: know each type of gateway and what purpose they would be used for.

FSx
Amazon FSx is a newer service and it is file server similar to EFS. Remember EFS is a shared file system for Linux and you can not use EFS for Windows. So AWS created FSx for Windows and it is a fully managed Windows file system share drive that supports the SMB protocol and Windows NTFS. It supports Active Directory integration and ACLs. It is build on SSD and is highly scalable  distributed file system for windows managed by AWS. It can scale up to 10 of GB per second and millions of IOPs and so on. It is highly availabe and can be configured for Mutli AZ. It can be accesed from your on premises, and your data is backed up daily to S3.

We also have another Amazon FSx for Lustre which is a type of parallel distributed file system for large scale computing. Lustre's name comes from Linux and cluster so that will help you remember it is for Linux instances and cluster is for the large scale computing.

EXAM TIP: Lustre is great for ML and High Performance Computing (HPC), you will probably see HPC on your exam a few times, Lustre has sub-milisecond latency.

Lustre is also great file system to perform video processing, financial modeling, design automation whatever needs a high-level of distribution. It seamlessly integrates with S3 and you can read your s3 buckets as a file system using fFSx Lustre and write computes back to s3.

Databases
RDS
RDS stands for relational database service, and RDS is considered a Database-as-a-service DBaaS.  RDS is an AWS service that provides managed database instances, and with RDS you are paying for and consuming a db server that we have access to.  AWS handles the management, and we get access to a managed db instance and this provides lots of benefits, and performance enhancements. We do not have to manage the physical hardware, the OS, and so on and RDS supports MySQL, MariaDB, PostgreSQL, Oracle, and Microsoft SQL Server, andAmazon Aurora. So you can pick which db works with your application requirements.

RDS databases come in different types, sizes, and families just like EC2 instances. RDS instances can be in one AZ or in multiple AZs.  For an RDS instance you allocate storage for that instance to use, so it is dedicated storage for that db instance.  And access to and for your db instances are controlled through SGs. RDS instances in a single AZ can be vulnerable to a failure in that single AZ because the instance and the storage are in a single AZ.

Multi AZ allocates secondary hardware in a different AZ. This second db instance is called the standy by replica instance. RDS uses synchronous replication from the primary and the standby instance.

With RDS you access your db instance by its CNAME and that CNAME points to the primary instance only, so you have no access to your secondary instance. You only have the single endpoint address pointing to the primary replica, you cannot use your standby instance for extra capacity etc, it only accepts synchronous replication from the primary instance.

The writes are committed to the primary instance replication to the standby at the same time. Now if for any reason our primary instance fails, RDS will detect this and change the CNAME to point to the standby instance. And this may add a brief interruption, but this failover provides HA and it automatic.

RDS read replicas provide two main benefits, performance benefits and availability benefits.

A read replica is a read only replica of your RDS db instance, and you can read replicas for read operations, and data is replicated asynchronously.  And asynchronous replication it is written fully to the primary instance first, and then it is replicated to the read replica, so there can be seconds of lag depending on your network conditions etc.  Synchronous replication is completed in Multi AZs and the data is written to the primary instance and replicated to the standby read replica at the same time.  So on the exam if you see asynchronous think read replicas and synchronous replication would be the choice for any question with a multi AZ env/scenario. Read replicas can be in the same region or different aws regions, if different aws regions it is cross region read replica. Read replicas are important bc they provide performance improvements.

If you have 5 read replicas per db instance with RDS, each of those read replicas provide and allow you to scale out read capacity for a db, so your application can perform reads against the read replica and not against the primary db instance. Then you can use the primary for writes only. You can create read replicas of read replicas but this adds lag and this lag can start to be a consistency problem. Read replicas also provide global improvements bc it scales reads; it is great for availability improvements, and offer global resilience bc you deploy read replicas all over the world.

We can use snapshots and backups to improve RPO, recovery point objective, and read replicas offer near zero RPO. This is done asynchronously from our db instance and if our primary fails then we can promote our read replica to be our new primary instance within minutes. This only works for failures bc read replicas will replicated corrupted data, and then at that point you could not use this as a failover, you would have to use a snapshot before the corruption.

RDS backups, snapshots, and restores

It is important to understand these RDS features bc not only will you see exam questions but you also need to make sure your data is secure, and you also need to understand these features for DR.

From our AWS Fundamentals we talked about DR and we learned about RTO, recovery time objective, and RPO recovery point objective. Remember that RTO is your recovery time objective, so it is the time between a failure and when you system is back online, and again lower rto is usually more expensive bc you need more resources

RPO is the time between when the last working back occurred and when the failure occurred, and it is the maximum amount of data you are prepared to lose, and the lower your rpo usually means more expensive, bc you need more backups and more resources

So with backups it is important to know your RTO and RPO requirements. For RDS we have two types of backups: automated backups and manual snapshots. S3 stores the backups/snapshots in S3 managed buckets. This adds to our backups, region resilience because remember S3 replicates our data across at least three AZs in a region.

Snapshots are manual snapshots that you take of your db instance, and again stored inside S3 similar to EBS snapshots. The first is a full copy of the data and then are incremental, and there is a brief interruption during your snapshots, and with single AZ there is impact but again on multi AZ there is no interference bc the snapshot is taken on the secondary db instance. It is important to remember that you must go in and delete your snapshots, you have to remember to delete those snapshots and if you delete your RDS instance or you will continue to pay for that storage. You can take a snapshot of your instance before you terminate your instance for good.

Automated backups are also snapshots and you choose the time of that backup window, the first is a full copy and then after they are incrementals. These are not retained and are automatically cleaned up and you can save these for 0 to 35 days before they are automatically deleted. You choose the retention period. DB transaction logs are written to S3 every 5 minutes so your db can be restored to a specific point in time.

As far as billing, you are billed for your RDS instance, an hourly rate for the compute and amount of storage that you allocate to your instance.  So like EBS you are billed on the amount of storage you allocate, not what you use.  It is a gigabyte per month metric for billing.

EXAM TIP:

Multi AZ

This feature is not available with the free tier bc you are using extra resources

RDS multi AZ does not scale your reads, it cannot be accessed directly and the standby provides not added performance, it is only good for HA.

Multi AZ is in the same region only - cannot be used across regions

Backups can be taken from your standby instance so backups have no performance impact or interruptions on your primary instance - backups in a single az will cause performance issues

Remember asynchronous is Read Replcias and they are for read scaling

Synchronous equals multi AZ for HA

RDS handles restores by creating a new RDS instance, with a new db instance endpoint address, so your application will need to be updated

When you restore a manual snapshot, you restore that db to a single point in time, and this can influence your rpo

Automated backups have transaction logs recorded are every 5 minutes

Backups are restored from the closest snapshot and transaction logs are replayed to bring the db to the desired point in time

Restoring snapshots is not fast, it can take a long time and is not always great for DR, bc that restore time influences your RTO, what will help is read replicas

But if you have data corruption you should use restore bc corruptions will be replicated to RR.

https://www.youtube.com/watch?v=igRfulrrYCo&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=7

Aurora
Aurora is a relational db and part of RDS, but it does have quite a few differences and improvements over RDS.

First the Aurora architecture is very different from RDS, Aurora uses the base architecture of a cluster.  And it compatible with MySQL and PostgreSQL engines. It is a cluster made up of a single primary instance and then zero or more read replicas. This may seem the same as RDS but Aurora read replicas can provide the benefits of reads and also the benefits of multi AZ. So they can be used to improve availability and read operations on your cluster.

Second, Aurora storage is different from RDS because Aurora does not use the local storage for the compute, it actually uses a shared cluster volume, which provides faster provisioning, improved availability and better performance.

You can have up to 15 read replicas with Aurora and each can be a failover choice. And since Aurora read replicas do not have the local storage like RDS, Aurora read replica can be added and removed without requiring storage provisioning, so it improves our speed and efficiency of our replica changes in the cluster. Each instance in your cluster receives an endpoint, remember for RDS only the primary db instance had an endpoint, but with Aurora each reader also gets an endpoint along with the primary cluster endpoints for writes. And you can create custom endpoints too.

Billing for this storage is based on what storage you consume,

Aurora cannot be used in the free tier

Compute is charged hourly and you also have a storage cost as well that is billed in GB per month consumed and your backups are included at 100% of your storage consumption

and with aurora provisioned single master we can have aurora serverless and aurora global dbs, and we will cover those in just a minuted

Backups in Aurora work the same as they do in RDS

Resotres create a new cluster

Aurora also offers BackTrack which must be enabled but allows you to roll back your database to a previous point in time, so no application configuration updates are needed, it is simply rewinded to that point in time.

Aurora also offers fast clones by referencing the original storage and only stores the differences between the two dbs.  Clone dbs only uses a small amount of data, stores data in the original after the clone and the clone itself.  Only the changes are stored bw the source databases and the clone.

Failovers, well when the cluster realizes there is a failure, then the primary failover to one of the read replicas, and this can take some time.

In a single master mode for Aurora you can have multiple endpoints. There is a cluster endpoint that is used for writes and we have up to 15 reader endpoints that are used to load balance the reads.  And with this single master the failover to a read replica can take a bit of time, because the reader has to be promoted to a read and writer.

But with multi master all of the instances in your cluster are capable of reads and writes, so the failover is much quicker. The same architecture exists, the difference is there is not a cluster endpoint to use, and there is no load balancer the application connects to one or both of the writer instances. When a multi master receives a write, the data received is sent to the storage cluster across all 6 storage nodes. With multi master the writers can also add that data to their in memory cache. For multi master failover, you have two writer instances, so if a writer fails then Aurora will simply send the requests to the one writer instance that is still working.  So it is much smoother and much quicker than in a single master architecture.

Aurora Serverless is a service of Aurora and provides a version of the aurora db product where you do not have to provision or manage the db instances. Aurora serverless works a bit differently architecturally. Aurora serverless provides the same shared cluster storage so you get again 6 copies of your data across three AZs. But we do not provision our cluster the same way, with Aurora serverless we use ACU which is aurora capacity units. The Aurora ACUs provide a certain amount of compute and a corresponding amount of memory. So for an Aurora serverless cluster we can choose a min ACU and a max ACU and then your Aurora serverless cluster will scale between that min and max value and will add and remove the capacity in your cluster based on the load. A really cool feature of Aurora serverless is the ACU can even go down to 0 and then can be paused after a period of inactivity so this is a great cost savings, because when your cluster is paused you are only paying for the storage that you are using. Billing for Aurora is based on the resources you use and are billed on a per second basis. You probably will not see Aurora serverless on your exam but I did want to cover it in case you do see questions on your exam.

Aurora Global dbs allow you to create global level replications and up to 5 secondary replications per region. It probably will not be featured on your exam, but again lets cover it at a high level. With Aurora global dbs, the primary region of a global db is very similar to aurora provisioned: you have one read and write instance and then up to 15 read replicas, but with Aurora global dbs, the second region's cluster is read only. You can have 16 RRs but again those are only read replicas, you do not have a writer instance. And replication is typically one second replication to the secondary regions which is sooooo fast and this replication occurs at the storage level so there is no impact on the db performance bc it is replicated at the storage layer.. And replication is only one way. Aurora global dbs are great for DR, and you can failover your primary cluster to your secondary clusters just like with provisioned Aurora. Aurora global dbs offer low latency and performance improvements if you have international users or customers.

DynamoDB (DDB)
DDB is a Nosql database as service product, and it is a public service and sits in the AWS Public zone. From the VPC section, we learned that we can use endpoints to access services inside the AWS public zone. So we can use the public internet to access DDB, or access it from inside a VPC with an internet gateway, or we can use a VPC gateway endpoint.

AWS manages DDB for us, we do not need to manage any servers or infrastructure and DDB can handle simple key value data or structure data. DDB also supports scaling options: using provisioned capacity with manual controls or use on-demand mode which handles scaling for us. DDB is highly resilient across multiple AZs in a region or you can configure a global table to add global resilience but this will be an extra cost.

DDB’s data is replicated across multiple storage nodes by default, and it is fast and backed by SSD. DDB also handles our backups, allows for point in time recovery, encryption at rest, and can support event driven integration to take actions if your table changes. Well, what is a table. A table is the base entity in DDB. A table is a group of items which all share a primary key, and items in that table is how you manage that data in the table. An item is like a row  and tables can have lots of items, there is no limit.

When you create a DDB table you have to pick a primary key and there are two types:

Simple (Partition) Key or Composite Key

The Simple Key is just the partition key (PK)
The composite key is a combination of the partition key and the Sort key (SK)
Every item in the table has to have the same primary key and it has to have a unique value for that primary key, but if the primary key is a composite key then the combination of the two parts the PK and the SK need to be unique in the table. And then your other items besides the primary key can have different attributes and this data can have all, a mixture, or completely different attributes. All items can be up to 400 kilobytes in size.

DDB can be configured with Provisioned or On-Demand capacity, and adding capacity means adding more performance, more speed, and so on.

On-Demand Capacity is handled for us, we do not have to set explicit values, we just pay for operations on our table, so cost per operation.
Provisioned Capacity is explicitly set on each table: write capacity units and read capacity units.
1 WCU = 1 KB per sec you can write one kilobyte of data per second to that table

1 RCU = 4 KB per second you can read 4 kilobytes of data per second from that table

DDB backups offer two types:

On demand and these are similar to manual RDS snapshots. DDB on demand backups are a full snapshot of our table that is stored until we delete that backup. It is stored in the same region or can be stored cross-region. It is a manual process, and you can adjust encryption and remember for cost savings to remove and delete the backups when they are n olonger needed.
DDB also offers point in time recovery and this type of backup can be enabled per table, and when enabled it is a continuous stream of backups of all changes to your table over a 35 day period. And you can restore anytime from any one second interval within that 35 day window if backups.
We can access DDB via the console, CLI, and API. Billing is based on the set RCUs, WCUs, and the storage plus any features you enable. You can use reserved capacity for an added cost savings but you do have the longer term commitment.

So remember we can choose between two different capacity modes when we create a table: on demand and provisioned. And you can actually switch between these two modes if needed.

On demand is designed for when you have an unknown design or unpredictable load and remember we do not have to explicitly set our capacity settings but this is more expensive than using provisioned capacity, you pay a price per million read or write units.
With Provisioned capacity you set a capacity value for our reads and writes on each table and those are rcus and wrus
And every operation on your DDB table will consume at least 1 RCU and 1 WCU

Capacity is rounded up, so even if you consume less than 1KB, it will round up to 1 KB

EXAM TIP:

1 WCU = 1 KB per sec you can write one kilobyte of data per second to that table

1 RCU = 4 KB per second you can read 1 block of data up to 4 kilobyte of data per second from that table

And each table has an RCU and WCU burst pool that equals 500 seconds of the read and write capacity units of our table, but this pool is also used by other table tasks, so try to reserve this pool when it is needed only.

EXAM TIP:

We can perform lots of types of operations on our ddb table but the two you will probably see on your exam are query and scan.

A Query is a way to retrieve data from DDB, and we use a partition key value to start this query, so we specify a single value for our partition key, and that will return an item or items. It is always more efficient to pull as much data as possible in one query, so we do not have multiple reads and waste our RCUs. We can also filter this down by adding a sort key value or a range of sort key values. So a subset of sort key values, we are billed for the returned data. And filters are charged for the entire size of the items, so it is best practice to minimize the size of your items.
And to perform more flexible operations we can use scan, however, it is not efficient for getting your data, but it is flexible. So you can choose a specific attribute or filter and those will be applied to our scan. And the scan moves through your table and consumes the capacity of each item in the table, so the entire table is consumed, but it will give you control on what data is selected. However, it does access every item so the whole table is consumed. It does not return items that do not match the attributes selected and added or the filter selected and add but it consumes the entire capacity of that table.
DDB also has two different consistently read modes. Consistency is the process of when new data is written to the db and then read, is that data the same as the most recent update or is it eventually the same.

Strongly consistent writes and Eventually consistent writes. Strongly consistent writes are more costly and do not scale well. Eventually consistency is easier to implement and scales much easier.

In DDB every piece of data is replicated in separate AZs, and each storage node in the 3 different AZs and one of these nodes is the leader storage node. So when our items are replicated across the storage nodes, and one of our items is updated, it is then written to our DDB table. Writes are directed to the leader node with the updated item, then the leader node is consistent because it has the updated data. Then the leader node will start replicating the updated item to the other storage nodes to also make them consistent.

With ddb we also have eventually consistent reads and strongly consistent reads:

Strongly consistent reads is 1 RCU = 4KB always use the leader nodes which is the first node updated.
Eventually cons reads are cheaper and you can read twice the amount of data on the same RCU.
So if we use eventually consistency then DDB directs us to one of the three storage nodes for our table, and the storage nodes usually have the same data but sometimes the writes are not updated and you could get older not updated data, so you will not always get the latest data but you get a cheaper price, so it is half the price of Strongly consistent reads but the data may be old.  It is not often but it can happen. But some applications cannot tolerate the eventually consistent reads, like stock apps, medical records apps, and so on.

How to determine our values for our capacity for our DDB table:

What if we need to store 10 items in our table every second. And the average size is 2KB

We first need to know the average size of our item and how many items per second will be written. If you have questions based on minutes, remember to switch the minutes to seconds bc that is whole we calculate our capacity.

So to calculate WCU per item = we take the item size 2.5KB) and divide it by 1KB = 2.5and round that up = 3

Then we multiple by the average number of items (10) per second (3) to get our calculations = 30 WCUs

Let's also look at read calculations, so to calculate the RCU per item =

So let's use the same example, so we need to retrieve

10 items per second and the average size = 2.5K

So we take the item size and divide it by 4 KB and then round up that number.

(item size/4KB) then round up .   (3/4KB)=.75, so rounding = 1

Multiply by average read op per second (10)=10 so 10*1=10

Strongly consistent  RCU = 10

But for eventual consistent read we divide the RCU value and divide it by 2

10/2=5 5 RCUs will be required

**These calculations will feature heavily in your Certified Developers Associate exam but you may get a question on your SA exam. But it is really good to have this understanding, but for the exam remember the size of an RCU and WCU for the associate exam.

Let's wrap up DDB and talk about DDB streams and triggers.  They can be valuable to cost optimize your DDB table. A DBB stream is an ordered list of changes inside your DDB table, so each change Is recorded in order to this DDB stream and a DDB stream is a 24 hour window of all changes, and can use Kinesis streams. You do have to enable streams on each DDB table, and you can configure your stream to have different views: keys_only, new_image, old_image and new_and_old_image. Streams can be used with db triggers so it allows you to take actions when changes in your data occur, and we can implement this in a serverless way. And this saves money because you do not have to poll your dbs and only consume the minimum amount of capacity required.

EXAM TIP:

Know that you can use DDB streams and Lambda to create triggers and can then take action.

If you see questions asking for NoSQL then the answer is probably DDB, NoSQL is a keyword.

If you see relational db in the question then it is not going to be DDB, DDB is a non relational db.

If you see key value in your exam question then DDB could be the answer.

If you see any questions with SQL or the structured query language then DDB is probably no the correct answer.

https://www.youtube.com/watch?v=skr_raPPvTc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=26

OpenSearch
Elasticsearch (recently changed to OpenSearch) not sure which name will appear on the exam

Amazon Elasticsearch Service is a fully managed service that enables you to search, analyze, and visualize your log data cost-effectively, at petabyte-scale.

Elasticsearch clusters are challenging to set up, scale, and manage. As a fully managed service, Amazon Elasticsearch Service manages the setup, deployment, configuration, patching, and monitoring of your Elasticsearch clusters for you, so you can spend less time managing your clusters and more time building your applications. With a few clicks in the AWS console, you can create highly scalable, secure, and available Elasticsearch clusters. Amazon Elasticsearch Service offers open source Elasticsearch APIs, managed Kibana, integration with Logstash and other AWS services, and SQL querying, so you can continue to use your existing tools and code.

Elasticsearch, allows us to search any field in a db, even partial matches.  ES allows you to build a cluster of instances, and it integrates with kinesis firehose, IOT, and CW logs, for data ingestions. It works great with DDB, but with DDB you can only find. Data with exact matches on the primary key or indexes, but with  ES we can search any field and partial matches too.

AWS secures ES using Cognito, IAM, KMS, and SSL and multi AZ clustering

EXAM TIPS:

And ES works great with Kibana for visualization

Cost is pay per provisioned node.

ES allows us to search any field.  It is great for searching and indexing.

RedShift
Redshift is a petabyte scale data warehousing solution form AWS, it is a column based db engine for analytical workloads. Most RDS dbs are used for OLTP, online transaction processing, but Redshift is designed for OLAP, which is an online analytical processing, and it is not the type of db where you update individual records, it is used for data warehousing analytics, and everything is stored in columns.  And column based dbs are great at queries because all data is in columns. Row based dbs are great for transaction type processing and column based dbs for analytics. Redshift is based on PostgreSQL but is an OLAP. Redshift is NOT used for OLTP. Redshift uses a cluster architecture and unloads and uploads data to S3. It can also accept data from DDB, Database Migration Service (DMS), other dbs, and Kinesis too. And to go along with S3 we can use Redshift Spectrum to perform queries directly against S3. This is not like Athena, with Redshift Spectrum you must have a Redshift cluster, but you do not need to load the data into Redshift: you can simply queries directly from S3. Athena is serverless so there is not an instance to provision.

Redshift also has point in time backups that are stored to S3, and snapshots are incremental and occur every 8 hours, every 5 GB, or on a schedule. And you can select a retention period.    Only the data that has changed is saved, and we can use the snapshots to restore to a new cluster. Redshift can also be used with DR, we can configure Redshift to automatically copy snapshots of our cluster to another AWS region. As far as cost, we pay for what we provision (so the instances we provision), per node provisioned. Also for cost optimization all manual snapshots are retained in S3 until deleted.

EXAM TIP:

Know that Redshift is a data warehouse used for analytical and summarization transactions, and can scale to almost any workload needed and is a petabyte scale db.

Elasticache
Elasticache, which is a managed in memory cache for performance improvements for reads.  It supports two different popular caching engines: redis and memcacheD. So if you see a question with memcached or Redis your answer is probably EC. EC is designed to store reads and deliver those results from in memory caching and improves performance, so instead of consulting the db each time for reads, you can cache results and then deliver those results quicker. EC can also be used to store user session states. And we mentioned sessions in the fundamentals section, but you can store the users session states using EC. And EC can be used as a performance enhancing tool or used with fault tolerant architecture.

You should not see too many questions on your exam but may see one or two.

DDB Accelerator (DAX)
Lets talk about DAX too because EC used to be used with DDB, but AWS created DAX to be used specifically with DDB. DAX is the DDB accelerator. As we learned earlier, DDB, is designed to be a low maintenance and high performing db that provides access to data in milliseconds, but we do have edge locations that need this data faster like microseconds, and also for high read sessions, and DAX provides an in memory cache for DDB.

DAX runs inside your VPC and uses a cluster architecture so we can have one or more nodes, and applications use a DAX client installed on the same resources as the app itself. So when items are read from DDB, the items are returned to the application, but also stored in DAX. And if that items is read again it is returned using DAX without using DDB. And that is called a cache hit, if it is not in DAX, then it gets pulled from DDB and is stored in DAX and is then returned to the application. And that is known as a DAX miss.

DAX is designed for latency sensitive and high read workloads

DAX also has two distinct caches: the item cache and the query cache.

The item cache is made up of results from GetItem and BatchItem and comes with a 5 minute default TTL, the query cache stores results of Query and Scan operations and caches the results based on parameters specified.

You can also use Elasticache/OpenSearch for DDB also, but DAX was specifically designed to work with DDB so it is the preferred in memory cache for DDB.

EXAM TIPS:

So you may see a question asking what is the best caching product to use with DDB and the answer is DAX.  Dax is NOT great for applications that need strongly consistent reads. Dax is more for eventually consistent reads.


High Availability and Scalability
Load balancers are used to achieve high availability, fault tolerance, and scaling. So let’s cover the essentials of load balancers.

So what is a LB? Load balancing is a method used to distribute incoming connections across a group of servers or services. And incoming connections are made to the LB, which then distributes them to the servers or services.

In AWS we have four choices for LBs, Classic (CLB), Application (ALB), Network (NLB), and the Gateway Load Balancer. And these four make up a family of elastic load balancers (ELBs) and they are great to pair with auto scaling groups to enhance the high availability, fault tolerance, and scalability of an application. For the exam know that LBs have listeners that listen for traffic protocols and ports. In AWS HTTP listens on port 80 and HTTPs listens on port 443 from users, and then behind the LB we have the app server/s. When a user connects to the LB, then the LB takes those requests and distributes those requests between the application servers.

The architecture is that connections are made from the client to the LB, and then the LB decides which instance to use. Then the LB makes a connection with the backend instance and sends your request to that instance or brokers that connection, but if you click on another link you might be switched to a different instance.

So there are two separate connections, one from the user's client to the LB and then another connection from the LB to the particular application server. And these two connections are called the listener connection and the backend connection.

When you create a LB you are creating one entity, one LB, but it actually creates an ELB node.  For HA, a LB node is placed in each AZ that a LB uses. And the ELB gets a DNS record that automatically points to the ELB nodes, and the connections are split between the nodes. For the exam know, you can enable cross zone LBing to allow each node to distribute traffic to all instances. And this is enabled by default.

LBs also run health checks against all servers, if one fails, then the LB will stop sending requests to that failed server.

LBs are great for HA, scalable and fault tolerant architectures. If you deploy an application rather than point the application to one or more instances, specifically you can simply point to a LB that has two or 50 attached instances.  That helps scale and also adds HA if an instance fails then the LB will send that connection to another instance.

Exam tips:

Clients connect to the load balancer's listener configuration, and then the LB connects on your behalf to one or more servers for the application.

ALB - Application Load Balancer
AWS started off with one type of load balancer which was an ELB, elastic load balancer. However, it did not provide a lot of features, so AWS added more features and created an ALB and then even more features were added and AWS released the NLB.

So the legacy LB for AWS, the ELB, is actually the CLB classic load balancer and with the ALB and NLB makes up the family of three products known as ELB. There is a newer load balancer that was added too, the Gateway Load Balacner.

Exam tips:

The ALB is known as a layer 7 LB from the OSI model, and at layer 7 this means that the ALB can inspect data that is passed through it and can understand the application layer, HTTP and HTTPS. The ALB can then take actions based on things in that proctol like paths, headers, and hosts.  And all AWS LBs are scablabe and HA.

And like we learned in the last lesson, the ALB is actually individual ALB nodes running in each AZ that is configured with your ALB.

So we did not mention this is the last lesson but LBs can be internet facing or internal, and the difference here is that internet facing have public IP addresses and internal LBs have private IP addresses. An internet facing LB is designed to be connected from the internet and LB those connections against the target instances, and internal LBs  are not accessible from the internet and are used to LB inside the VPC or between tier of a multi tier applications.

And again it listens from the outside and sends that traffic to targets or target groups. ALBs are billed at an hourly rate and an addition of the loadbased on the load placed on your ALB.

And remember ALB can also perform health checks across all its targets / instances. If one instance fails, then the target state for that instance will move to unhealthy and the ALB will no longer send requests to that instance.

So when you design the ALB architecture, you will see that ALBs have different services they can send requests to that are called targets .

So targets can be EC2 instances, containers in ECS, lambda functions, and so on. Targets are then grouped into target groups, and individual targets can be members of multiple target groups. And ALBs send requests to these target groups. So with ALBs you define listeners and rules that can be host rules or path rules.

NLB - Network Load Balancer
As we mentioned in the last lesson, ALB is recommended because it supports the functionality of the CLB and also supports layer seven protocol, HTTP and HTTPs, but what do we do if we need to load balance protocol that is not HTTP and HTTPS? We need the packets to remain untouched, so we need to support a protocol that is not web or secure web. It needs to be highly performant and put the packets through to the destination without any modification, well this is when we would use NLB and they operate at layer 4 of the OSI model. NLB and they do not touch that data in packert above layer 4. We can support other protocols as long as it utilizes TCP or UDP.

Exam tips:

NLB has advantages over ALBs.

NLB does not need to worry about the upper layer protocol, it is much faster.

It is able to handle high end workloads and scale to millions of requests per second.

We can allocate static IP addresses so it is easier to integrate with security and firewall products.

NBL supports routing requests on multiple apps on a single ec2 instance

And supports the use of containerize apps.

ALB is great for high end layer 7 protocol support
NLB supports any other protocols and can handle millions of requests.
So if you get a question asking which ELB can handle millions of requests then NLB should be your answer.

CloudFront
You should see CloudFront (CF) feature heavy on your certification exam, so let’s cover everything you need to know.

CF is the content delivery network in AWS. It is a global object cache, content delivery network or CDN, so instead of your global customers connecting directly with your application or content server, with CF, your content is cached in global locations that are as close to our customers as possible.

So if the content is cached in CF locations then it is directly delivered to your customers,if not then it is fetched, cached and then delivered to your customer.

So CF brings lower latency for your customers and higher throughput, so faster page loads and interactions with the apps.

CF can handle both static and dynamic content.

So lets cover CF concepts before we see the CF architecture bc it is important to understand terms and know what they mean as a fundamentals but also we need to know these for the exam and for real world too

Origin is the original location of your content. This can be an s3 bucket or an ALB or anything on the internet as long as CF can access it.

Distribution is the unit of configuration in CF, so we have to configure a distribution and then this distribution is deployed out to the network.

Edge locations are the global infrastructure where your content is cached. There are more edge locations than regions and AWS currently has over 200 edge locations throughout the world.

And we also have regional edge cache, and these are larger and hold more caches than the edge locations. There are not as many spread throughout the world.

CF integrates with the AWS Certificate Manager(ACM), so you can use CloudFront to add HTTPs capability to your statically hosted website running on our S3 bucket. AWS Certificate Manager is a product that lets us manage and deploy public and private certificates to use with AWS services. Certificates allow HTTP sites to handle encryption and allow it to prove its identity. HTTP is a simple and insecure protocol, so new server identity authentication or transport encryption was built into HTTP, but security vulnerabilities became an issue, so HTTPs was designed to address these security vulnerabilities. HTTPs uses SSL/TLS secure tunnel. It adds a layer of encryption and data is encrypted during transit and allows identities to authenticate, with the certificates we prove our identity and are trusted as a signed authority

So ACM creates and renews and deployed certificates to AWS supported services, like CF and ALBs, usually managed AWS services are supported with ACM.  But not EC2.

And if we use a certificate with CF or an ALB, then that communication from our users and the edge locations are encrypted, and the edge locations will communicate with the origin using the protocol configured. BUT if your CF distribution is set to communicate between the edge locations and the origin using HTTPs you need a trusted signed certificate.

CF is only for download style operations only but does support uploading content with five additional http methods, POST, PUT, DELETE, OPTION, AND PATCH. But when content is uploaded CF sends the upload request back to the origin; CF does not cache writes. You may see a question around this on your exam. CF does not handle any writes caching.

And CF can be configured to be private, so if you are using a private CF distribution then you need to prevent direct access to your bucket bc making CF dist private will only affects access via the edge locations, so users can access the bucket directly using the buckets dns then the CF restrictions will not apply, so make sure you removed direct access for your bucket.

What if we want to make sure that users cannot directly connect to our s3 bucket, and we want customers to use CF and the edge location. We can create an OAI and this is an Origin Access Identity. Once created we can associate this identity with a CF distribution, and this will give our edge locations this OIA ID. We can then add a bucket policy to allow the OAI, and remove any other explicit allowances for the bucket policy, remember only one bucket policy can be attached to a bucket at a time. So once this is completed all access from the edge location will be the OAI ID from our edge locations and S3 will know this is from the OIA /edge locations and access will be allowed but any other access will be denied. OIA can be used on CF distribution and buckets at the same time but it is best practice to create an OAI for each distribution.

Global Accelerator
Let’s discuss the global accelerator which adds lower latency for users. We just covered CF but what is the AWS Global Accelerator? We need to know both for the certification exam.

The AWS Global Accelerator uses the AWS global network to route the application and instead of using the public internet. And it is a service that is used to improve the availability and the performance for your users. The GA uses the public internet until we hit that edge location and then uses the AWS global network. So our traffic is sent to the closest edge locations through the private AWS network but without the AWS GA your traffic/packets will take different hops.

And the AWS GA works with elastic IP addresses, EC2 instances, ALBs, NLBs, and GA can either be public or private. It offers intelligent routing to lowest latency and fastest regional failover. Uses health checks to perform health checks on your application, and is also great for DR. With AWS Shield which we will cover in an upcoming lesson we can use AWS GA and AWS Shield to offer DDoS protection.

So what is the difference between CF and GA because they both use the AWS global network and the edge locations. Both also integrate AWS Shield for DDoS protection.

But here are the differences:

CF will improve content for cache content both static and dynamic content and content is served from the edge locations most of the time.

GA improves the performance for applications over TCP and UDP because the packets are being proxied from the edge locations to the apps running in one or more regions. So all requests are making it to the edge and there is no caching available. GA is great for HTTP use cases that need a static IP, or need fast regional failover.

Route 53
Let’s do a high-level overview of Route 53. So what is Route 53? Well, it is AWS's managed DNS (Domain Name System) product and it essentially helps us with two things: first we can register domain and second Route 53 can host zones on managed nameservers.

Route 53 is a global service with one single database and it is replicated between regions - making it a globally resilient service - meaning that it can tolerate the failover of one or more regions and continue to operate. It is a huge hierarchical database

DNS is a service used to help discover other services on the internet.  And it translates addresses from the language that computers understand to the language that humans understand and then back again. So if we want to go to amazon.comwe type in amazon.com, but computers use IP addresses, so DNS translates our words into IP addresses and then finds that location; it then sends that location back to us and translates the IP address back to words that we can understand.

The two main functions of Route 53 that we mentioned: Registering Domains and Hosting Zones.

Route 53 can register domains and is able to do this bc Route 53 has a relationship with all of the major domain registries: .com, .edu, .uk. .org, and so on.

Route 53 can also be used as Hosted Zones and also provides DNS zones and hosting for those zones. So route 53 is basically DNS as a service. Remember a Route 53 hosted zone is a DNS DB for a given section of the global DNS data for domains.

A hosted zone can also be private and linked to one or more VPCs and only accessible inside those VPCs.

Hosted Zones host our DNS records and record sets, and again that is A record, alias record, cname record, and so on.

Simple & Multi-Value routing policies
Let’s cover Route 53 routing policies. Routing policies are how route 53 responds to queries and which records get returned when users query domains. Route 53 offers simple routing, multi value, failover, weighted, latency and geolocation routing policies.

Simple routing policies work by configuring standard DNS records without special route 53 routing. So if we want to route traffic to www.amazon.com it is a single resource, so that query flows to the hosted zone database and that database has one record www. Which could have three values, and then all three of those are forwarded back to the client and one of the values one of those records is chosen at random and then the website is accessed.

But sometimes one of those records could be unhealthy so you user would receive an error instead of being directed through to the website.

And with simple routing policies, you cannot perform any granular health checking but you can with other routing policies and Multi value routing offers a solution to simple routing.

Multi value routine policies are similar to simple routing; however, simple routing has a key difference that you can have multiple records with the same name and each of these records can have a health check. So Route 53 will respond with all healthy record IP addresses so you get multi values but will remove any unhealthy records, so no unhealthy records make it through to your customer.

Multi value offers a solution to simple routing, but it is still a single record (set) that may have more than one value (record); by attaching health checks you can return only healthy values.

Failover routing Failover routing policies
Failover routing, you actually create two records with the same name and the same type and one is the primary and the other is the secondary

It is very similar to the simple routing policy that only has one record with one name. But with failover routing we have two records with the same name: so our primary record in this example could be a wordpress EC2 instance and your secondary record could be an EC2 instance or it could be the S3 endpoint URL from our S3 bucket hosting our static website. And we could use that S3 bucket for a static hosted error page; we would simply need to copy the S3 endpoint url.

So the point of failover routing is that if anything happens with our wordpress site that we created on our EC2 instance, then the route will failover to our secondary wordpress EC2 instance or even our S3 bucket hosting our ss static website.

And with failover routing we use health checks and each record has an associated healthcheck, so if the primary route is healthy then it is the one used. The secondary is only used when the primary record's health check fails.

Failover routing is used to implement active passive failover in DNS.

So with simple routing we cannot create multiple record sets with the same name but with failover we can And failover is great for HA.

Weighted routing policies
Weighted routing is a powerful routing policy and the way it works is you create multiple records with the same name within the hosted zone; however, each of those records you apply a weighted value, so maybe 50 50, or 75 25, or 90 10.  Weights can be assigned any number from 0 to 255. And the total percent weight is all the records added together and how often each record is returned on a DNS query is based on how heavily it is weighted.

And again you can use health checks so weighted routing policies are great for active/active failover, great for deployments; so you can add smaller percentage of request coming to the new application to see how it handles traffic and then eventually up that weight if it is working as needed and then remove the weight from the older application version.

And weighted routing is a really useful technique for all kinds of deployments. AWS give us multiple ways to do this: DNS is one of them, but we'll also see similar in EC2 load balancing.

And for simple traffic distribution, if you have services on a smaller EC2 instance, you can reduce the weight of traffic to that instance and have more weight going to a larger EC2 instance.

If you have migrations, it allows you to gradually move you load over.

Latency routing policies
Latency routing allows you to create multiple records with the same name and the same type.

For each record you specify a region for that record, and when a client request arrives, route 53 knows what region that request is coming from and also know the latency of that region and other regions as well and it will pick the healthy record with the lowest latency.

Latency Routing is a Public-Hosted Zone thing. It's possible to create within a private hosted zone, but doesn't really do anything. AWS has the ability to predict the likely latency for users based on their source IP address as long as it is a publically-routable address.

And I can add a like if you want to take a deeper dive.  More here: https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resource-record-sets-values-latency.html

It is not based on geography, it is not a distant thing, it is based on latency.

Geolocation routing policies
Geolocation routing is focused on delivering queries to match the location of your customers, the physical geography. So you can create records with the same name and type in a hosted zone, but set a location field, so that location can be default, set to a country, or continent. So when a users queries for a record, Route 53 locates the location of that customer and then tries to match that location to a record in that county, if it cannot then it will try to achieve a continent match, and if cannot do either of those, then the default record if no other record applies is returned. If no record is located in that geolocation and no default record is listed then nothing is returned

If the records have a health check and the records are in an unhealthy state it will simply be passed over to the next record. Geolocation is designed to offer localized content to your customers by returning records in their geographic area, so those records can be in different languages to match those countries, etc. and priority also goes to the most specific record

A use-case of this is data protection/sovereignty issues for example Europe's general data protection regulation - and Geo-routing would be a great reason to use geo-location (as opposed to latency) to ensure the right EC2 instances, and databases, interact with European customers.

Types of DNS Records: CNAME vs Alias
A & AAAA
CNAME
TXT
MX
NS
In this lesson let's talk about the types of records that can be stored in DNS and Route 53. Without taking a deep dive it’s important to know that A and CNAME records are standard DNS records, whilst ALIAS records are custom DNS records.

A records

A records or AAAA records -  map host names to IP addresses,

A records map to IPv4 address and AAAA map to an IPV6 address

CNAME records, canonical name, for a given name the cname creates DNS short cuts, so host to host records. So if we have an A records pointed at our EC2 server for ss.com and maybe this server serves our website and performs multiple tasks, also receive emails from users, etc. so you can create three cname records to point to the one ec2 server A record, so all three CNAME resolve to the same IP address and CNAMEs can reduce your admin overhead. But CNAMEs cannot point directly to specific IP addresses only to other CNAMES or records.

Alias records

Amazon Route 53 alias records provide a Route 53–specific extension to DNS functionality. Alias records let you route traffic to selected AWS resources, such as CloudFront distributions and Amazon S3 buckets. They also let you route traffic from one record in a hosted zone to another record.

An alias record can only redirect queries to selected AWS resources, such as the following:

Amazon S3 buckets
CloudFront distributions
Another record in the same Route 53 hosted zone
For example, you can create an alias record named acme.example.com that redirects queries to an Amazon S3 bucket that is also named acme.example.com. You can also create an acme.example.com alias record that redirects queries to a record named zenith.example.com in the example.com hosted zone.

Understanding the differences

These are the main differences:

The A record maps a name to one or more IP addresses
The CNAME record maps a name to another name. It should only be used when there are no other records on that name. If the IP of the destination hostname changes, you won’t need to change your DNS records as the CNAME will have the same IP.
The ALIAS record maps a name to another name, but can coexist with other records on that name.

Important rules:

The A, CNAME, and ALIAS records cause a name to resolve to an IP. The A name must resolve to an IP. The CNAME and ALIAS records must point to a name.
MX Records are huge bc they help email on the internet work, so if you want to send an email, MX records are used as part of this process, so your email has to know what server to pass this email along to. MX records have a priority and a value, and the value can be a host or a fully qualified domain name, so it can point to a host in the same zone or to an outside zone, the priority value is used to choose which value to use

MX records use the SMTP protocol to deliver the mail

TXT records are also know as a text records and these allow you to add text to a domain, so the dns can provide additional functionality, and txt records can be added to our email to prove we own that domain

https://www.youtube.com/watch?v=HKh54BkaOK0&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=9

https://www.youtube.com/watch?v=6R44BADNJA8&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=8

Application Services
SQS
Let’s cover Amazon's Simple Queue Service, SQS and what you need to know about SQS for your exam. So what is SQS? Well, it is a queuing system that provides fully managed highly available message queues and SQS can be used for inter-process, servers, and services messaging.

So the way a que works, if you have a que, you add a message to the que, and then something else retrieves messages from that que, so it offers an asynchronous way to talk between two components of an application.

Exam tip: You may see a question in your exam regarding the sizes of SQS messages and each message can contain up to 256 KB of data.

And SQS has two types of polling, short and long polling.

Short polling is a single API call to check the que for any messages, and you will get the messages available in the que up to a max of 10 messages or you will get no messages. With short polling it responds immediately to any messages in the que, meaning you will need to constantly be sending API calls to check the queue for messages, and this consumes a lot of API calls.

But you can also use long polling, and this is the same process to check for messages in the que as short polling; however, you wait for a certain amount of time, and that time is known as the WaitTimeSeconds. So with long polling you can specify a time you are willing to wait until that que has messages, and then when messages arrive in your que, during the WaitTimeSeconds, those messages will be delivered to you immediately so you do not have to keep short polling that que for messages.

And long polling is more efficient because you have a lot less API calls to the queue but also a lot less empty API calls.

So when you have a message that is polled from the que, it is hidden in that que, they are not deleted, they are simply hidden for an amount of time, known as the VisibilityTimeOut, and when this time out periods expires: let’s say our visibility timeout period is 1 minute, then that hidden message will return to the que and then that message is visible to the que again after the time period.

So it is best practice to delete the message from the queue after that message has been polled and processed, and you may see a question regarding this in your exam.

SQS queues come in two different types: Standard and FIFO Queues

Standard was the AWS original and Fifo queues were added later but there are a few differences to know for your exam.

Standard queues are distributed and scalable to nearly an unlimited message volume, but the order of the message is not guaranteed, it is best-effort, and messages are guaranteed to be delivered at least once, but sometimes the messages are delivered more than once. You can have duplicate messages or out of order messages, but have great performance.

FIFO queues were introduced to solve this problem. FIFO stands for first in and first out and FIF ques guaranteed that messages are delivered in the order they were received, they are only ever  delivered once, so dupes do not occur.  BUT the throughput is limited to 300 messages without batching and 3000 messages per second with batching.

So let's talk about SQS' architecture, and SQS is used when you need to decouple two different parts of a system, and decouple is an exam keyword, so if you see decouple, asynchronous messaging, or the ability to have independent scaling of your application, on your exam, the correct answer will probably be SQS.

https://www.youtube.com/watch?v=8zysQqxgj0I&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=13

https://www.youtube.com/watch?v=o4clRJuH9xU&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=11

https://www.youtube.com/watch?v=EBSdyoO3goc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=10

Logging and Security
Still to complete

Lesson Links:

iOS Google Authenticator : https://apps.apple.com/au/app/google-authenticator/id388497605

Android Google Authenticator : https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en_CA

1Password : https://1password.com

Authy : https://authy.com/

Let’s secure our new AWS account. Now remember we talked about how our AWS account begins with a single root account user, and remember this user has full permissions to this AWS account and that these permissions cannot be changed.

What we did not talk about is how much of a risk this is, because if our account root user creds are compromised then our whole AWS account is too. So when we logged into our new AWS account remember we added the email address and the password for our root user. And if anyone besides you provides both of these correctly, then they can log into your AWS account as the account root user with full admin creds.

So we want to secure our account permissions so no one, but ourselves can log in as the account root user and take control over our AWS account. And a way we can do this is by adding multi factor authentication to our AWS account. So currently we have an email address and password that is known, so that is considered One Factor. And honestly email addresses are usually pretty easy to figure out. So that would just leave the password. And it is best practice to use MFA and add multi factor authentication to your AWS account and also your users in your AWS account. This adds more security bc MFA not only uses the email address and password that you know, but also adds another factor to enter to log into the AWS account. It uses a one time password also known as OTP, that actually changes on a regular schedule. An MFA can be attached to users inside our AWS account, even our account root user, and once attached in addition to the email address and password, now we also have to provide an OTP, so a one time password that the MFA device generates for us.

So all three will be needed to log into the AWS account. And by using an MFA it makes our aws account more secure because the code changes each time, that code is only valid for a very short time, and that OTP you are given can only be used one time.

Walk through for setting up an MFA on our account root user.

open console

In the AWS mgmt console on the right hand side, let's open the drop down under our account name and select my security creds. And you will see it takes us to the IAM console, the Identity and Access Management console and we will be discussing IAM later on in this section. But you will also see we have security creds and we are being asked if we want to configure our security creds or get started with IAM users.

But we want to configure our security creds, so click, and now we want to open up MFA to activate our MFA. When you see the blue button, click it and now we get to choose the type of MFA device to assign. Choose a virtual MFA device, and click continue. Now we need to download the google authenticator app if you do not already have it, check the links above. Make sure to click show QR code and then you simply scan this QR code with your application. And then the application will begin generating OTP one time passwords for you to enter here below. So you need to enter one code and then wait for the new code to appear and then enter that as well, so you will enter two consecutive OTPs, and then click on assign MFA.

Now we have assigned a virtual MFA to our AWS account and now our root user is more secure.

We will be creating new IAM users, specifically a new admin IIAM user that we will start using instead of our current account root user. That is AWS best practice to use the account root user for your account set up and then only for emergencies. Remember, the root user has full permissions to your aws account. Before we wrap up, another best practice is to enter alternate contacts for AWS to contact you and I always enter my personal info here bc it makes it easier for aws to contact you with any emergencies. There is also the option to add IAM users the ability and permissions to access billing reports, etc. This is a personal choice that you can decide to check the box or not. For my own account I do not want others having this access but again the choice is yours.

Create a Billing Alarm
https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/monitor_estimated_charges_with_cloudwatch.html

https://www.youtube.com/watch?v=3peNAKB3VxA&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=36

Along with the AWS Free tier, we can create a billing alarm to be notified if we are exceeding a monthly budget. Most of the services you use with AWS are set up so you pay for what you use, or also known as on-demand billing, and services are billed differently in AWS. Some are billed:

per second

per hour

per gig, and so on.

So one important cost optimization tip to know how you are charged for the AWS services you use. And also know that some AWS services offer discounts for a bigger payment up front. But whatever you choose to use, you do pay for that usage each month.

Now AWS offers an amazing option to use the AWS Free tier for a new AWS account for a 12 month period. And the AWS Free Tier is a service that gives you free access to different AWS services, and this is a great tool to use because you can gain free hands-on experience with the different services.

With the AWS Free Tier, you get:

EC2 - 750 hours per month
S3 - 5 gig of standard storage
RDS - 750 free hours
Lambda - 1 million free requests per month, and so on.
So make sure when you are designing your architecture that you understand the free tier usage is different for different services so make sure you have an understanding of what is needed and what is offered for free.

IAM Intro
Identity and Access Management (IAM) is a core AWS service you will use as a Solutions Architect. IAM is what allows additional identities to be created within an AWS account - identities which can be given restricted levels of access.

IAM identities start with no permissions on an AWS Account, but can be granted permissions (almost) up to those held by the Account Root User.

Right now in your AWS account, you only have our account root user that has full permissions to the AWS accounts. And remember it was created when we created our account and we cannot adjust the permissions for our account root user. But in most cases you will want to grant other people in your organization permissions inside of your AWS account. You will have your different users like your storage team, engineers, sys admins that will need access to the AWS account and also access to the services in your AWS account. It is AWS best practice to practice the principle of least privilege which means only giving access to users in your AWS account to the specific services that they need access too. So users in your account only need permissions to do their job, they do not need any other permissions.

So remember earlier we mentioned reducing our blast radius and another way to do this is too use the principle of least privilege and make sure users in our AWS accounts have the permissions needed but nothing more. So how do we control access to our AWS account and the AWS resources inside the AWS account? Well, this is where IAM comes in and saves the day! Now before we get started with the intro of IAM, I have another EXAM TIP and that is that every AWS account comes with its on copy an IAM which is a database and IAM is a global AWS service that secures any data in the aws iam db across all AWS regions so you can think of IAM as a database service and can do almost anything like your aws account root user.

So let's take a deeper dive into IAM, and IAM allows us to create identities in our AWS account. IAM Users, IAM Groups, and IAM Roles.

IAM users: IAM users represent people and also applications that need access to our AWS account. And you may be thinking really Julie, applications? And yes, sometimes applications need to log into our AWS account to access certain services. And it is important to know for the exam , that IAM identities start with no permissions on an AWS Account, but can be granted permissions needed. IAM Users are one of the identity types available inside AWS. They are the type you pick when you can identify a single individual or 'thing' which will use that identity - a person, an application or a service account. How to create an IAM user in your AWS account?
IAM groups: IAM groups are simply groups of related users, such as your Dev team, your SysAdmins, your storage engineers, and so. And you can even have a group for your finance team to check your usage, and spend of your account. An IAM group is a collection of IAM users and helps to manage IAM users and groups and organize large sets of IAM users. IAM groups have no creds of their own, so groups do not have creds and you cannot log into an IAM group. You may see a question on your exam asking you if you can log into a group and remember that you cannot. You may also see a question asking if an IAM user can be a member of more than one group and the answer is yes. An IAM user can be a member of 10 groups. But there is no limit to how many users can be in a group. If you have an organization of over 5,000 people and you create a group to include everyone in the company, well all 5,000 plus could be added to a single group. But you would have to create that group, and then add the users to that group. There is not a built-in group for all users. Users by defaults have no permissions until we explicitly grant those permissions. There is a soft limit of 300 groups per account but this can be increased with aws by opening a support ticket. EXAM TIP: groups are not true identities like IAM users and IAM roles. They are both considered identities, groups are not. So groups cannot be referenced in an IAM policy because they do not have an Amazon Resource Name (ARN). So IAM policies or even resource policies cannot grant access to an IAM group. A resource policy is a policy on a resource that can reference IAM users and IAM roles using the ARNs. And you may see AS try to trick you on your exam with a question regarding this.
IAM roles: IAM roles are used by AWS services but can also be used to grant external access to your AWS account. For example you would need to grant an EC2 instance inside your AWS account access to CloudWatch, S3, or other services. A role is one type of identity inside our AWS account and the second is IAM users. An IAM user is a single principal. An IAM user is a single thing, a person, an application; it is a single identity needing access permissions in our AWS account. An IAM role is also an identity in AWS. But an IAM role is used by multiple principals, so this could be multiple AWS users, applications, services, inside your AWSaws account, but these could also be users, applications, and so on outside of your AWS account too. So if you are unsure how many principals would need these permissions, then it is probably a good candidate for an IAM role and not an IAM user. And remember that you could use a role if you hit the 5,000 user limits for IAM users. IAM roles are also usually temporary, and roles are assumed. So you assume the permissions/that level of access inside the AWS account and then become that role. And when you stop using those permissions you no longer assume that role, IAM users have long term creds. A role does not represent you like an IAM user does. A role is a level of access or a thing you can use to get the needed permissions. SO with a role you are using permissions for a short period of time; you become that identity for a short period of time.
IAM policies: IAM also has IAM policies. We use IAM policies to allow or deny access to our AWS services, and IAM policies are a bit different because an IAM policy has to be attached to an IAM user, an IAM group, or an IAM role. So you can use AWS Managed Policies or you can create a new policy, and again that policy will simply allow or deny access. On their own policies just sit there, to take action they must be attached to a user, a group, or a role. IAM policies and how aws handles the security of their users and resources. IAM policies are policies that get attached to identities inside of AWS just like we attached the aws managed admin access policy to our admin user. EXAM TIP: identities in AWS are IAM users, IAM groups, and IAM roles. As a solutions architect you will use IAM policies a lot, and you need to understand IAM policies for the certification exam. Two crucial things you need to know for your exam is 1)understand how policies work, how they are designed and architected. 2)Be able to read policies and understand what that policy is allowing or denying. 3) And then I am going to add in a third but it is not required for the exam but it is something you should work towards, and that is to be able to write your own policy, and this third comes with practice and time. More on policies and permissions
So on a high level overview, IAM acts as an ID Provider, or IDP, and it manages identities inside your AWS account, it also authenticates these identities to be allowed to log into your AWS account, and then authorizes those identities to access resources or deny access to resources bases in the policies attached.

Now as far as cost optimization for your AWS account, IAM is free to use, there is no cost, but there are limits to how many users, groups, and so on, you can create.

EXAM TIP: For the exam, you may see some limitation questions on IAM limits, remember it is a global service, it is resilient. You can only have 5,000 users per account. And an IAM user can be a member of 10 groups.

IAM provides identity federation so AWS allows authentication using AD, google, amazon, and facebook.
It allows us to secure our AWS account using MFA.
IAM identities start with no permissions on an AWS Account, but can be granted permissions needed.
IAM Policies - deeper dive
So what is an IAM Policy? Sometimes you may see them referred to as an IAM Identity policy but they are both the same thing.

It is a set of security statements that grant access or deny access to AWS resources, products, features, and so on.
An IAM policy consists of an IAM Policy Doc that is written in JSON.
There are two types of IAM policies:

AWS Managed Policy
Inline Policy
Both are the same as the policies we have been discussing but the management is different between the two types.

Inline policy is a policy you create and then apply that policy to individual users. And inline policies are not best practice, but in small envs they can be used. Inline policies are managed individually, so you have to update each inline policy that is attached to users in your account. An advantage of an inline policy is that they are great when you have a special exception to one individual that needs a different set access than anyone else or maybe needs to block access to one user. So remember special or exceptional allows or denies as a reason to use inline policies.
AWS Managed policies are much easier to manage. An AWS managed policy is created with just one version of the needed JSON policy doc, and then you attach the policy to any users that need it. If this policy needs updating you only have to update the one AWS managed policy. If you update an inline policy, then again you must update that policy for each user that uses that policy. Another advantage of AWS managed policies is that you can reuse those policies. And AWS managed policies have two types:
AWS managed policies are managed by AWS.
Customer managed policies are policies we create and manage ourselves.
IAM Roles - deeper dive
IAM roles have two types of policies that can be attached, the trust policy and the permission policy. A trust policycontrols what identity can assume the role. So the trust policy must allow the identity to assume the IAM role. Trust policies can represent IAM users, other IAM roles, and also AWS services, but it can also reference identities in other AWS accounts as well as facebook google, etc.

So if an IAM role gets assumed by something that is allowed to assume it from the trust policy, then AWS will generate temporary security credentials and give those back to the identity assuming the role. And these temporary creds are time limited and only work for short periods of time. When the identity assumes the IAM role with the temp security creds, then it is given access to whatever is allowed inside the PERMISSIONS POLICY.

When you assume a role the temp security creds you receive are generated by an AWS service called Secure Token Service / STS, and you may see an exam question asking what is the operation used to assume a role and that is sts:AssumeRole, you do not need to know the exact specifics or how it works but should remember that name just in case you have an exam question. And if you have a question with sts:AssumeRole you will know that IAM roles are involved. And these temporary creds are time limited and will then expire, but you can renew creds by re-assuming the role. These temp creds can access whatever permissions are in the permission policy

Trust policies can reference IAM users, other IAM roles and also AWS services, but it can also reference identities in other AWS accounts as well as facebook google, etc.

And remember since roles are real identities in AWS just like IAM users and roles can be referenced in resource policies with the ARN for s3 or ec2 and other services.

So lets cover common uses for IAM roles in our AWS account, and the biggest one is for AWS services themselves. So why is this? Well, when we use AWS services, we must explicitly grant those AWS services access and permissions to perform tasks and actions in our accounts. So when we choose to add an AWS service to our account, by default that AWS service has no permissions to act in our account. So the AWS service needs a way to get permissions to do whatever actions you are needing that service to do.

We can create IAM roles that these AWS services can assume with the needed permissions. And the IAM roles will have a trust policy as part of that role like we just saw and that trust policy trusts whatever service we are configuring permissions for. For example, we have an ec2 instance and we need that ec2 instance to log logs into s3. In this case, we would be creating an iAM role for the ec2 instance. That iam role would have the trust policy that trusts the EC2 service. So whenever ec2 needs to send logs to s3, then ec2 can assume this role and use that role to have the permissions needed to put those logs into s3. This IAM role that we create remember also has a permission policy that grants access to services.

Back to our example, our ec2 instance when it needs to put logs into s3, it will use the sts:AssumeRole operation that we talked about earlier and the secure token service to generate the temporary sec creds for our ec2 instance and then ec2 can use the temporary creds to access s3 based on the permissions inside the IAM role's permission policy.

Now if we did not use an IAM role for this access we would need to hard code the security creds on the ec2 instance with the access keys needed. This is not AWS best practice or security best practices. This is a huge security risk because if those access keys are exposed then anyone would have access to do anything. It also causes problems if you ever need to change the access keys. But another EXAM TIP: it is always best practice to choose an IAM role because the service receives temp sec creds to perform the task and it really secures your env vs hardcoding creds. You will most likely see an exam question regarding how to add permissions to aws services and you should make sure to choose iam roles.

IAM roles can also be used when you want to reuse your existing identities from your on premises env and access AWS resources. BC you cannot directly access AWS resources with an external account. However, there is a process that allows you to allow users to use the external identities to access AWS resources.

How it works: you allow an IAM role inside your AWS account to be assumed by an external identity which may be in your on premises Active Directory. It works the same, when the role is assumed by the external identity: temp creds are generated and passed to that external user. And the reason this is important is because AWS accounts only allow 5,000 users per account. If you have more than 5,00o users you would not be allowed to create an IAM user for each of those. Plus that would be a lot of time consuming work plus lots of mgmt of 5000 extra users. But allowing an external identity to assume an IAM role, is called ID Federation and that means using IAM roles with ID federation to give you a smaller number of roles to manage vs over 5,000 iam user accounts. And the external IDs can use these roles to access the needed aws services.

IAM roles are also great for applications that need to access a database in your AWS account because users using a mobile application are most likely going to hundreds of thousands of users, and remember we have the 5,000 user per account limit. But we can use web identity federation and IAM roles for this situation. Most mobile apps allow you to sign in using FB, google, or amazon and the way this works is that our IAM role's trust policy trusts these identities from FB, google, and amazon and again they will then be able to assume that IAM role, they will be given temp sec creds, and then they will be allowed the permissions granted in the permission policy. And by using IAM roles the application has no hard coded creds stored in it which makes the app much more secure and also makes your resources secure as well. And it also uses the customer's existing accounts on amazon, fb, or google, so the user does not need to create a new account. EXAM TIP: You may see a question on your exam asking how to architect solutions for mobile apps and using Web ID Federation along with IAMroles is the way to do that.

AWS Organizations
AWS Organizations is an AWS product/service that allows larger business and smaller ones to manage AWS accounts with very little management overhead and in a cost effective way. Ok, great but what does this solve, how does it work?

Well without AWS Org it can be difficult to organize and track and manage multiple AWS accounts. Imagine companies that have many AWS accounts. Most large organizations break up their AWS account into multiple AWS accounts: An AWS account for dev and test, one for production, one for security, etc. So in this case, each AWS account has their own IAM users, resources, and so on, but also a separate payment method, because remember each AWSaccount is tracked and billed for the services used to the credit card info you enter when you create the aws account.

So the way it works is from one single AWSaccount, you create an AWS Org, and that account with AWS Org in it becomes the master AWS account of your AWS Org. Then from this master account you can invite other existing AWS accounts into your AWS Org, so they will be sent an invite and those AWS accounts must accept the invite to join your AWS Org. And when they accept the invitation, then those AWS accounts become part of the AWS Org as member AWS accounts. So the way AWS Org is designed is that they can have one master AWS account and then zero or more AWS member accounts. You can also create new AWS accounts from your AWS Org with just a valid email address and if you add accounts this way there is no need for the invitation to be sent, and then also accepted.

The AWS Organization has a root organization similar to our IAM account root user, but it does not have anything special besides acting as a container to hold other AWS master account and or other AWS member accounts.

It also can contain other containers known as Organization Units or Ous, and then these Ous can contain the master and member accounts or other nested organizational units.

So AWS Orgs added simplicity to managing all of your AWS accounts by basically grouping up different accounts to match your business organization AND it also gives you the ability to consolidate all of your AWS accounts into one bill, called consolidated billing. So instead of receiving 5 to 10 individual AWS account bills, AWS Org allows you to consolidate all of your AWS accounts into a single bill. The AWS member accounts pass their billing info to the master account which is the payer account. And this single consolidated bill covers the usage for the master account along with the usage for the aws member accounts.

Another awesome benefit of using AWS Org is that some AWS services get cheaper the more usage that you use, and other aws services are cheaper if you reserve that service and pay in advance for your usage, and with AWS Org, all of these services and usage is pooled for all AWS accounts in the AWS Org, so the all accounts can benefit from the combined cost savings.

You can also use IAM roles to allow access throughout the org to access other AWS accounts in the org. You do not need to create separate IAM users for each AWS member account. And you can use IAM roles, specifically IAM role switch to interact with other accounts

AWS Org has a feature that restricts what member accounts in the org can do and that is called a Service Control Policy SCP. A SCP policy is a JSON policy doc that can be attached to your AWS Org as a whole by attaching the SCP to:

The root container
One or more OUs
One or more AWS accounts directly.
So an SCP inherits down the org structure. If an SCP is attached to the :

AWS Org, affects all accounts in that org.
OU, then they affect all accounts in that OU, and the accounts below that OU.
One or more accounts, then they just affect those accounts.
SCPs are permission boundaries and limit what the accounts can do, including the account root user of that account. So if you have an SCP in your account that prevents usage of an AWS service, then nothing in that account including the root user can use that AWS service. SCPs can limit activity outside of a particular Region, or that allow a certain type of ec2 or rds instance, and so on.

SCPs are used in two main ways:

To block services by default and then allow certain services and this is known as an allow list
Allow by default and block access to certain services known as a deny list.
The default for AWS org is to use deny lists, so allow services by default, and then block access to certain services.

So when you enable SCPs on your AWS Org, AWS will apply a default policy called Full AWS Access for your AWS Org. This policy allows all AWS access, so basically the SCAP has no effect because nothing is restricted and everything is accessible. Again SCPs do not specifically grant access they only control which permissions can be granted, BUT when SCPs are enabled there is an explicit deny, just like IAM policies.

Create an AWS Organization
How to create an AWS Organization

IAM Access Keys
So far in this content, we have only been dealing with AWS access using the console, but we can also access our AWS resources using the CLI and also access resources using apis, sdk, etc.

However, unlike authenticating to the AWS management console, authentication with the CLI does not use our user name, password, and MFA. We authenticate with the CLI using IAM access keys, and like our username and password, access keys are also long term creds,

An IAM user can have two sets of access keys but only one username and one password

So access keys can be created, they can also be deleted, made inactive, and made active.

And an access key is made up of two parts:

Access Key ID which acts like your user name
Secret Access Key which acts like your password
So the Access Key ID is public and the Secret Access Key is private just like a username is public and the password is private. And AWS gives you both of these when these creds are created, but once created, AWS will then discard your Secret Access Key, so it is crucial to copy your Secret Access Key and keep it somewhere within reach but safe. AWS does not store your Secret Access Key, so if you do not copy it and keep it somewhere safe you have no other option than to delete that access key and create a new one.

And that wraps up our AWS Fundamentals section. Next we will dive into a new section covering Network and Compute in AWS.

Networking and compute

VPC Default Structure
Hi and welcome to a new section on networking and compute and we are starting with Amazon VPCs, let's start off this section and look at the AWS default VPC that AWS provides for all their AWS accounts.

Earlier we talked about the essentials of VPC, so now I want to talk specifically about the default VPC in your AWS Account. So again a VPC is a virtual private network, and it is a service that we use to create private networks in AWS. Our private services will run from this VPC. We can also connect our VPCs from our AWS private network to our on premises for a hybrid environment, or you can connect to other cloud platforms when you are creating a multi cloud env. VPC is a huge part of the certification exam.

When you create a VPC, it is in one region in one AWS account, so this makes a VPC a regional service. And VPCs operate resiliently by operating in multi AZs in a specific AWS Region. By default your VPC is isolated and private until you explicitly grant public access, but there is one exception and you need to know this for your exam and that is the default VPC.

There are two types of VPCs in AWS: the default VPC: you can only have one default vpc per region and also custom VPCs.

Custom VPCs are configured by us as we need them, we are responsible for all of the configurations and by default are isolated and private.
Default VPCs are created by AWS when you create your AWS account and AWS sets up the configuration for us.
Each default comes with one VPC CIDR Range, which is a given range of IP addresses and this VPC CIDR defines the start and end range of the IP address that this default VPC can use. So everything inside your VPC uses this CIDR range, all communications to the VPC will need to use the VPC CIDR and outgoing communications will be from this VPC CIDR. All default vpcs are configured in the same way.

And with your VPC you can divide your network across the azs for resilience, so you can sub divide your VPC into subnets and subnets is short for sub network. Each default VPC is configured to have one subnet located in each AZ of that region. And each subnet in your default VPC uses part of the IP address range of the VPC CIDR. And each subnet's IP address range must be unique to the other subnet’s IP address range and also cannot overlap. So if one of your AZs fails, then that subnet in that failed AZ will also fail, but with the default VPC you have other subnets in other azs that are still operating.



EXAM TIPS for default VPCs:

You can only have one default VPC per region, it can be deleted and then recreated
You can addIPv6 CIDR but you must enable your VPC for IPv6
The IPv6 CIDR for your subnet range is /64 and the VPC CIDR range is /56
And the local route is used to communicate between subnets inside your VPC
The default VPC CIDR is always the same and designed and configured the same too 172.31.0.0/16 is the default VPC CIDR
/20 for the subnets in each AZ in the region and subnets are assigned public IPv4 address, so they are all public subnets and will be in the aws public zone
And each Default VPC will be provided, an IGW, SG, and NACL
Networking Intro
Lesson Links

https://www.iana.org/numbers

https://en.wikipedia.org/wiki/List_of_assigned_/8_IPv4_address_blocks

Private Addresses RFC1918 https://tools.ietf.org/html/rfc1918

Prefixes : https://www.ripe.net/about-us/press-centre/understanding-ip-addressing

https://www.iana.org/numbers

Before we get too far along in our VPC section, I do want to do a highlevel overview of networking because you may see questions on your exam.

So let's start with the Internet Protocol, known as IP, is how devices communicate in AWS and over the internet. And there are two Internet protocols, IPv4 and IPv6. IF you are interested in a deeper dive into Networking Fundamentals in AWS, check out my YouTube channel.

So IPv4 addresses are represented by dotted decimal notation which consists of four numbers from 0 to 255 separated by a period and the bit between the period is called an octate.

It starts with 0.0.0.0 and ends with 255.255.255.255 giving us over 4.2 billion IP addresses, and this is a large range, but we are running out of IP addresses because these days people have laptops, mobile phones, tablets, etc.

This range was split using classful addressing into smaller ranges

The first range was called Class A and it starts at 0.0.0.0 and ends at 127.255.255.255so that was over 2.1 billion ip address
Then we have Class B and this range starts at 128.0.0.0 and ends at 191.255.255.255 and gives a little over 1 billion ip address
Then we have Class C and this range started at 192.0.0.0 and ends at 223.255.255.255 and gives a little over 2 million ip address
There are also Class D and Class E ip ranges but they are not included in the aws certification exam, so we will focus on Class A,B, and C.
These IP addresses are publicly routed IP addresses, so you can connect to them.

There were also ranges created for private networks to be used in private networks or in AWS

And these IP addresses cannot communicate over the internet they are private. And these IP address were broken down into ranges too:

Class A is 10.0.0.0 - 10.255.255.255 One single Class A
Class B is 172.16.0.0 - 172.31.255.255 16 Class B
Class C is 192.168.0.0 - 192.168.255.255 256 Class C
And our default VPC in AWS is configured in a Class B

So for private IP addresses to communicate with the internet they have to use NAT which is network address translation and we will be covering that a bit later.

This classful process was eventually replaced with CIDR which stands for Classless Inter-Domain Routing. And CIDR removed the limitations of being limited to class A,B, or C size networks.

CIDR addresses are represented by the starting IP address of the network called the network address and the prefix which is a forward slash and a number that represents the size of the network.

So a CIDR looks like this 10.0.0.0/16, so the starting address of the network is 10.0.0.0 and the size of the network is a /16 and for the certification exam you do not need to know much more than a high level of networking, but I will added links above if you are interested you can take a deep dive bc understanding this early on will definitely help especially when you decided to take your AWS Advanced Networking Specialty exam, but for the CSA exam try to remember that the bigger the prefix, the smaller the network, and the smaller the prefix, the larger the network.

So back to our 10.0.0.0/16 will provide a total IP addresses of 65,536

And with CIDR we can split up these IP addresses to create different networks. So we could split it into 2 networks which would be two /17, or 4 networks which would be /18, and so on. This process is called subnetting.

0.0.0.0/0 means all IP addresses, it is the biggest of all networks. So everything
And you may see a slash /32 on your exam. A /32 means 1 IP address. /32 is the smallest network possible
A /8 gives you 16 million ip addresses and is a class A
A /16 gives you 65,536 Ip addresses and is a class B
And a /24 gives you 256 IP addresses and is a class C
IPv6

An IPv6 address is much longer and is represented in hexadecimal rather than the decimal like IPv4 addresses. And is 128 bits long And is called a hextet and because the address is so long we can abbreviate the address by removing redundant zeros.

And the IPv4 networks are also represented by using the start address and a prefix, but with IPv6 each hextet is 16 bits and the prefix number is actually the number of bits that represent the network part of the IPv6 address.

Double colons represent unneeded zeros, so ::/0 means all IPv6 addresses and you may see this on your exam but definitely in AWS.

Subnets
Subnets are what services run from inside our VPC, and they are how we add structure and functionality to our VPCs, and remember that subnets are an AZ resilient feature of AWS.

A subnet is a subnetwork of our VPC CIDR range. And it is created in one AZ, and because it runs in one AZ, if that AZ fails then so will our subnet and the services running inside the subnet. And this is why we need to design our infrastructure for high availability. EXAM TIP: that one subnet is in one AZ, and it can never be in more than the one AZ. But one AZ can have 0 and more subnets. The certification exam may try to trick you on this one, so remember 1 subnet = 1 AZ.

You may have a question on your exam asking what is the IPv6 CIDR subnet range and that is a /64 and the IPv6 cidr range for your VPC is always a/56.

Subnets in your VPC can communicate between each other using the local route.

One thing we did not mention in our intro to networking section above is that some IP addresses inside each VPC are reserved, so we are not able to use those addresses.

And there are 5 ip addresses in each subnet that we cannot use,

The first address that we cannot use is the first address of each network 10.0.0.0
The second address is the Network +1 address and this is the first IP address after our Network Address, so this IP address would be 10.0.0.1 and AWS uses this address for the VPC Router
The third IP address that we cannot uses is called the Network +2 address, so the second ip address after our network address, and AWS uses this ip address for DNS 10.0.0.2
The fourth address that we cannot use and this is the Network +3 address and it is reserved in case it is needed, 10.0.0.3
And the last address we cannot use is the broadcast address which is the last IP in our subnet, 10.?.?.255
So if we should have 16 IP addresses, then we would only actually have 11 IP addresses that we can use, so that is important to know when you are designing smaller VPCs.

Also subnets have a DHCP option set which stands for dynamic host control protocol. This is how computer devices receive their IP addresses automatically, and each VPC comes with one DHCP option set, and can only have one applied at a time, it can be changed BUT for the exam know if you need a new one you must create a new one, you can not edit your DHCP option set.

Routing and Internet Gateway (IGW)
Every VPC has a VPC router that is highly available, and simply moves traffic from somewhere to somewhere else and it runs in all the AZ that your VPC uses. The router has a network interface in each subnet in your VPC and uses the Network+1 address we discussed. You never need to worry about this router, it just works and it's managed by AWS, and routes traffic between subnets in your VPC. We can control this router a bit by creating route tables and associate the route table with the subnet and add rules to allow traffic in and out of your subnets.

Each VPC has a main route table (RT) associated with your subnets, so if you do not explicitly associate your RT with your subnet, then the VPC will use this main RT. A subnet can only have one RT associated with it at a time, but you can use one RT for many different subnets in your VPC.

RTs are created at the VPC level but they are associated with a subnet, which is in one AZ, and only one RT is associated per subnet at a time.

The IGW is a regional resilient service. So it is highly available, and sits on the edge of our VPC and the AWS public zone and the internet. It manages traffic between our VPC, the AWS public zone, and the internet, and the reason we only have one public RT is that the IGW is per VPC, so one IGW works across all AZs.

IF you create a new IGW, you must attach it to the VPC, it is not automatically attached. Then add a route to our RIGHT to allow traffic to and from the IGW. If we add an IGW route to a subnet then it becomes a public subnet because it has access to the aws public zone and the open internet.

The IGW does this by performing a type of NAT called static NAT, and how it works is that the IGW allocates a resource with a public IPv4 IP address. So when the data or packets leave that resource and pass through the IGW, the IGW switches the source IP address from the private IP address to the public IP address and sends the packet on. Then when the packet returns, it switches the destination address from the public IP address back to the private IP address.

Network Access Control Lists (NACLs)
Network Access Control Lists (NACLs) are a type of security filter (like firewalls) which can filter traffic as it enters or leaves a subnet. NACLs are attached to subnets and only filter data as it crosses the subnet boundary. NACLs are stateless and see initiation and response phases of a connection and 1 inbound and 1 outbound stream requiring two roles (one IN one OUT). You will most likely get a few questions on NACLs on your exam.

And by default a default NACL is created for your default VPC associated with all subnets by default.

NACLs are used for traffic entering or leaving a subnet bc NACLS are associated with the subnet not with resources. NACLs only maange traffic that is crossing the subnet boundary. If you have two EC2 instances in your VPC that are communicating, NACLs will have no involvement because the communication between the two instances are not crossing the subnet boundary.

NACLs are stateless and what that means is that if you add a rule for inbound traffic, then you must also add the same rule for outbound traffic. NACLs only see the traffic going one way, so if you allow an inbound rule then you must also allow an outbound rule, so your NACL will explicitly see that traffic that was allowed inbound is also allowed out. NACLs see the traffic as two different streams so you must have two rules, one rule for each stream. IF you do not add your outbound rule, then the traffic will only be allowed in.

NACL rules are processed in order from lowest rule number to the highest rule number, when a rule is matched, an action is taken, and processing stops. An important EXAM TIP is that NACLs can have allow rules or deny rules, and NACLs can explicitly allow or deny specific IP addresses.

All IP communication is actually made up of two parts, the initiation part and also a response part. And a lot of the time, the response part does not use the same port in its response, but instead uses the ephemeral ports. And the ephemeral port range is ports from 1024 - 65535

So with NACLs it is important to remember to add the ephemeral port range.

EXAM TIPS:

NACLs are Stateless
NACLs only affect traffic crossing the subnet border, only applied to the subnet
NACLs can be used to explicitly allow and explicitly deny traffic
NACLs only support IP, Networks, and Protocols, you can not add AWSresources or services
Use NACLs with SGs to add an explicit deny
One subnet is associated with one NACL
NACLs are processed in ordered, so lowest number to highest and ending with the * which is for everything
Security Groups
SGs are another security feature of AWS, only unlike NACLs that are attached to the subnet, SGs are attached to the elastic network interface (ENI) of the AWS resources in the subnet. They also work differently than NACLS. SGs are assigned to the ENI of an AWS resource, so it sits at the boundary, per se, of the instance instead of the subnet.

SGs also have inbound and outbound rules, but SGs are stateful. That means that if traffic is allowed in, then that traffic is automatically allowed back out. SGs see both the inbound and outbound traffic as part of the same stream. One big difference between SGs and NACLs is that SGs recognize AWS resources and you can add rules for these. For example, for an EC2 instance you could add:

The instance ID for that instance to allow traffic from the instance
Rules for other SGs, or add a rule for the SG itself.
SGs also have a hidden explicit deny which means that anything that is not explicitly allowed is denied. BUT for the exam make sure understand SGs cannot explicitly deny a certain IP address, like a NACL can. If you need to explicitly deny, then you need to use NACLs. You will probably see an exam question on this.

EXAM TIPS:

So when would you use NACLs and SGs?

NACLs are used with subnets
NACLS are used for explicit denies
SGs are used for almost everything else and are simpler bc they are stateful there are less rules needed to secure your env
NACLS again are associated with subnet, not with EC2 instances communicating
Custom VPC
Let's cover a few differences between your default VPC and your custom VPC. Your custom VPC is also a regional service like your default VPC. It is an isolated network. And nothing is allowed in or out without explicit configuration. Custom VPC are completely configurable by us. We can create a hybrid network to connect our AWS VPC with our on premises network, and our custom VPC has a choice for default or dedicated tenancy. Default tenancy is resources provisioned inside your VPC that are provisioned on shared hardware with others. Dedicated tenancy is the hardware that is dedicated to you AND dedicated tenancy will be much more expensive. Custom VPCs can use IPv4 CIDR blocks and public IPs and we are given a private IPV4 CIDR block when we provision the VPC. Remember the networking overview, we can choose the largest CIDR range with a /16 - 65,536 IP addresses or the smallest /28 - 16 IP addresses. With your custom VPC you can also have an optional secondary block of IPv4 addresses.

We can also configure our custom VPC with a single assigned IPv6 /56 CIDR block. (we do not get a choice with IPv6 like we can with IPv4). IPv6 are all public IP addresses by default.

Custom VPCs also have fully provisioned DNS, and remember that is the Network +2 IP address. And for the exam you should remember to enableDNSHostnames, then your instances in your VPC will be given public DNS names. You should also choose enableDNSSupport to enable DNS resolution in your VPC. You may see questions relating to either on your exam.

Bastion Hosts
I want to add a high level overview of bastion hosts, also known as jump boxes. We will be covering these under our EC2 instance, cloud compute section. A bastion host is simply an Ec2 instance in a public subnet inside a VPC. And they are a great security feature that can be used to allow incoming management connections into private resources in subnets. It is an inbound mgmt point and you can really tighten up what access is allowed with your RTs.

NAT Gateways
Network Address Translation (NAT) is the process of giving a private resource outgoing access to the internet. TIGW performs a type of NAT called static NAT by allocating a resource with a public IPv4 IP address. When the data or packets leave that resource and pass through the IGW, the IGW switches the source IP address from the private IP address to the public IP address. And then sends the packet on. When the packet returns, it switches the destination address from the public IP address back to the private IP address. So NAT gives a private CIDR range outgoing internet access and to the AWS public zone. And when private resources initiate traffic with a NAT Gateway, they can receive responses back in BUT outside traffic from the internet can not initiate traffic inbound.

AWS provides us two ways to use NAT, using an EC2 instance or by using a NAT Gateway.

Why might a private service need access to the internet? Well the most common reason is for software updates. So software updates are needed, but they also need to stay isolated and private. You can configure your private RT to have a route to the NAT GW, and then configure your public RT to send this traffic from our NAT GWY out. And like the IGW, the NAT GW works in a similar manner;

When the private instance sends data to the NAT GWY, it does so using the RT to the NAT GW from the private RT, the NAT GW then records and stores the source address of the instances sending this packet and also records the destination address that the packet is for. (it can do this for multiple different instances too, in a translation table) Then it adjusts the packets and changes the source address of the instance to be its own source address, the NAT GWY source address, and then uses the route to the IGW to send the packet. The IGW takes the packet from the NAT GW, and then modifies the packet to the NAT GWY public address.

The NAT GWY allows multiple private addresses to masquerade behind it. By using the NAT Source address and then eventually the NAT GWY public IP address that the IGW gives it. So to give private instances access to the internet, you need both the NAT GW and the IGW to complete this and also to configure the routes for the route table.

EXAM TIPS:

NAT GWYs have to sit inside a public subnet bc it needs a public IP address
NAT GWYs also need updated RTs to allow routing
NAT GWYs use elastic IP addresses, an EIP is a special type of IPv4 addresses that are static and do not change.
NATGWs are an AZ resilient service, so for HA you need to add one NAT GWY into each AZ that your VPC uses, update the RTs too for each AZ
NAT is not required for IPv6 bc all IPV6 addresses are publicly routable and the IGW can work directly with IPv6 addresses
NAT GWYs does not work with IPv6
I do want to mention egress only gateways because we just mentioned that NAT GWYs do not work with IPV6. You do not need a NAT GWY for an instance in a private subnet that needs to communicate with the internet for software updates, etc. Because with IPv6 addresses, they are publically accessible and they can communicate with an IGW in a bi-directional manner.

The IPv6 instance can communicate with the public internet and the public internet can communicate with that instance. We can use egress-only gateways instead of NAT GWs for IPv6 instances that we do not want the public internet to be able to access these private instances directly.

With an egress-only gateway, the private instance in a private subnet can communicate with the internet, so it has a route outbound from the instance to the internet. And then that outbound traffic allows the inbound response. BUT with an egress-only gateway, the public internet cannot initiate traffic inbound to this private instance inside the private subnet. So it is an outgoing only version of an IGW for IPv6 instances. Outgoing only that is why it is called egress-only.

VPC Peering
VPC peering is a way to link multiple VPCs together and allows direct communications between two isolated VPCs using their private IP addresses. VPC peers can span AWS accounts and also Regions, and the data shared is encrypted using the AWS global infrastructure.

EXAM TIPS:

Use NACLs and SGs to control access
Why would we use VPC peering?

VPC peering is great for shared services running in a single VPC and you want those shared services to be accessible to other VPCs
To connect your VPC to a vendor or partner system to access an application or in reverse
To give access to your VPC, during a security audit
To meet requirement to split up an application into multiple isolated VPCs to limit the blast radius

https://www.youtube.com/watch?v=6fhwoAwYrug&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=28

VPC Endpoints
VPC endpoints are gateway objects we can create inside our VPC, sort of like IGW and NAT GWYs. They are used to allow instances inside a VPC to connect with AWS public services without the need of a gateway. An IGW or a NAT GWY is not needed. There are two types of endpoints that we need to know the the certification exam:

Gateway Endpoints - A gateway endpoint is used for AWS public services, remember that some AWS services are public services and they sit inside the AWS public zone. Sometimes we want to connect to these public services like S3 or DynamoDB from a private instance or subnet that does not have access to the internet or a NAT GWY set up. Gateway endpoints can be restricted using policies, use routing and need an entry on the RT.

Interface Endpoints - Interface endpoints are used for everything else, and you have to pick the correct endpoint depending on the AWS services. Interface endpoints use security groups, not policies. They also use DNS with a prefix list.

VPC PrivateLink may also appear on your exam. It is an endpoint service that solves the problems of needing to expose an application to other VPCs in other AWS accounts. You could make the application public but then you are using the internet and all is exposed. You could also set up VPC peering, but that is a lot of management overhead and VPC peers must be set up to each VPC. VPC Peering will also expose other applications in the VPCs to the other VPCs. So instead you can configure a PrivateLink. It is the most secure and scalable way to expose a service to 10s or 100s of VPCs and does not require VPC peering, IGW, NAT GWYs, and so on.

If you see any exam questions asking you to expose VPC services to multiple VPCs, the answer is most likely PrivateLink.

https://www.youtube.com/watch?v=iu0-o6hiPpI&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=27

VPN
I want to change the direction of building our custom VPC and talk about connectivity options between our AWS VPC and our on premises networks. AWS has a service, AWS VPN, and it is a service that lets us configure a hardware VPN which is a HA virtual private connection between our VPC and on premises networks. Virtual private networks, VPNs, use the public internet as a transit route for on premises to your VPC. VPNs offer a fully encrypted route from wherever your on premises network is located to your AWS VPC.

So for the exam we need to understand architecture but also when we would want to use VPNs.

And there are three different architectures to know for the exam:

NO HA- A single tunnel between a virtual private gateway/tunnel endpoint and the customer gateway and this does not provide any HA bc if any part fails then we would lose this connection
HA in AWS - Full resilience has two tunnels from the single customer gateway, so we are connecting from a single customer gateway to two tunnel endpoints/virtual private gateways located in different AZs. Dual tunnels do require dynamic routing, so keep that in mind when you are designing your architecture.
Full HA - Here we are creating two customer gateways connecting to two virtual private gateways/tunnel endpoints. Each has two tunnels to the virtual private gateway/tunnel endpoints from the customer gateway. So four tunnels total.
EXAM TIPS:

Remember the three architectures- no HA, HA in AWS, and Full HA
AWS VPN can be set up in minutes, versus Direct Connect that takes months and we will discuss this next
VPNs are fairly cheap, per hour cost and an outgoing data charge that it is a bit higher than Direct Connect, but VPNs are good for lower data transfer requirements
Performance can be limited by your customer gateway router
VPNs offer encryption end to end
VPN performance is variable bc it uses the internet so you can have latency issues
You may get a Route propagation question: local route take priority, then longest prefix, static routes take priority, any routes from Direct Connect over BCP, static VPN routes, any VPN propagated in learned from BGP.
Direct Connect
We just discussed hardware VPN connections. We also have another option to connect our on premises networks and our AWS VPC. And that is Direct Connect (DX). DX is a dedicated physical connection between your on premises network and AWS. Remember a VPN connection is a virtual private connection over the public internet.

DX is a physical piece of fibre running between your on premises network and AWS's network. AWS has a number of direct connect locations that are distributed globally. To get a DX connection, you must have equipment located at one of the DX locations or a deal with a DX partner that already has equipment set up at one of the DX locations.

So DX is a physical or cross connect connection between an AWS router and another router. You can order a DX connection directly from the AWS console.

Once the physical connection is installed and operating we then have to design virtual interfaces (VIFs). And there are two types of VIFs, public VIFs and Private VIFs.

Public VIFS allow you to connect from your on premises network through to any public AWS services, S3, DynamoDB. SQS, SNS, and so on.

Private VIFs allow you to connect, it is a private connection, from on premises to your VPC. These connections are configured much like you configure your VPN connection. Need to create a virtual private gateway, attach it to a VPC, and then create the private VIF and associate it with your virtual private gateway. And then it operates a lot like a VPN at this point.

So if we want to connect to multiple VPCs, we do not have to repeat the above steps, we can create a DX Gateway. It does have to be in the same account but can be in different Regions and the VPCs cannot have overlapping CIDRs. But when you connect to multiple VPCs, the VPCs using the DX gateway does not allow VPC peering with the other VPCs. It only allows connections back and forth between the on premises and individual VPC.





EXAM TIPS:

When you need speed and consistency choose DX because DX has dedicated connections that do not share speed or bandwidth
DX runs over a private cable straight into the AWS network
DX offers low latency bc it does not use the public internet
Bc it is a physical connection, it cannot be configured quickly like the VPN, DX does take at least a week if you already have equipment in the DX location or months if you do not
By default it is not encrypted, BUT VPN is
It is not HA, it is one piece of cable, and equipment in the DX location
You can run a VPN connection along with a DX connection for HA or provision two DX connections for HA
You can always create your VPN first while you are waiting for your DX to become active, and you may see a question on your exam around this
VPC Cost Optimization
I want to wrap up our Network section and talk about cost optimization techniques for your VPC and networking. As we mentioned earlier in AWS fundamentals, it is so important to establish your account structure first. But if you already have an AWS account and you are trying to implement cost optimization, that is awesome!

Remember with your account structure you have defined metrics and goals to track with a business design to achieve the optimal outcome that you or your organization needs to be successful. And make sure you are using cost optimization design principles to design your infrastructure.

Remember to enable Cost Explorer and use the AWS Billing and Cost Management dashboard to track your expenses and usage. Enable tagging and enforce tagging.

EXAM TIPS:

Make sure your EIPs are attached bc you are charged for EIPs not attached in your env
Monitor your data transfer, most data transfer inside a VPC is free and data transferred out is charged.
And remember the fifth pillar of the AWS Well-ArchitectedFramework: measure and monitor your infrastructure. And this is crucial because your infra will most likely be changing, so you need measures in place to monitor and measure your usage and your costs. It is crucial to define your metrics, set target goals, define and enforce your tagging strategy, use cost allocation tags, and make sure you review regularly for any infra changes.
EC2 intro to resilient, elastic, and scalable compute systems
What is EC2 and what does it provide? Well, EC2 is virtualization as a service, it is an infrastructure as a service or IAAS product, and it provides so much value to our AWS accounts.

So, what is virtualization? It is running one or more operating systems (OS) on a piece of physical hardware known as a server. Each OS is separate, along with their applications, and also allows multiple different privileged applications to run on that same hardware using software to make their calls. And this virtualization started off with two different designs and then has kept evolving.

Emulated Virtualization (EV) was the first design of software virtualization. With this design the host OS still ran on the hardware along with a hypervisor that had additional capabilities. And then on top of this was a guest operating system that is known as a virtual machine and then each VM was windows or Linux and had a virtual allocation of resources: CPU, memory, and local disk space. VMs also have other devices mapped to them like network cards, graphic cards, and so on. And to make a long story short, the part of EV to understand is that these guest operating systems believe they are real, not virtualized, and also that they are running on real hardware. BUT this design was very slow because VMs had to talk directly to the hardware.
So Paravirtualization (PV) was created to work on an OS that can be modified. With PV the guest OS is still running in the same design, but instead of calling to the hardware, the OS is modified to have privileged calls become user calls. Those calls are then made to the hypervisor instead of the hardware. So the calls are passed to the hypervisor instead of the hardware, which is quicker and with PV, the OS almost becomes aware of its virtualization which improves the performance.
Virtualization then changed the design, and Hardware Assisted Virtualization was introduced. And in this design the CPU knows it is virtual and contains instructions and additional capabilities to allow the hypervisor to directly configure and control that CPU virtualization. So when privileged calls are made, those calls go to the CPU and then are redirected from the OS to the hypervisor because the OS still believes it is real. Remember the VMs believe they are real, for example, the VMs believe they have a physical network card but what they actually have are logical devices that use a driver that connect back to a physical piece of hardware on the host OS. And this process does consume CPU cycles on the host and can impact the performance.
But there is a last design where the hardware becomes aware of the virtualization, so the network cards and so on. This design is SR-IOV, Single Root IO Virtualization. And the way SR-IOV works is that it allows add-on cards like our example above, a network card, to present itself as mini cards instead of one single network. And as far as the hardware for the VM is concerned, these are fully unique cards and are presented to our guest OS as real cards for its own use, so no translation is needed for the privileged calls. And with EC2, you can use SR-IOV to meet enhanced networking requirements like faster speeds, low latency (even with higher loads), less CPU usage, etc.
EC2 instances are virtual machines, so the OS and also resources: memory, storage, CPU, and so on run on EC2 hosts which are the physical hardware / physical servers that AWS manages. EC2 is the default AWS compute service.

And the EC2 Hosts are either shared hosts or dedicated hosts.

Shared Hosts are the default for EC2 hosts that are shared among different AWS customers, and the customers do not get any ownership of the host hardware. You pay for your individual instances and resources, but it is important to remember that when you use a shared host, your instance is isolated from other AWS customers.
With Dedicated Hosts you are paying for the entire EC2 host, not just the instances you run on that host. You do not share it, you pay for the entire host , no matter how many ec2 instances you spin up.
EC2 instances are an AZ resilient service, because the EC2 hosts sit in an AZ, so if that AZ fails, then the host and the instances running on the host also fail.

EC2 hosts that sit inside an AZ also have local storage, called Instance Store. And the key to understand with Instance Store is that it is temporary. If your EC2 instance moves off the host to another host, then your storage for that instance store is lost. And for networking, you will hear that security groups are attached to your EC2 instance, but this is not necessarily true., The way it works is that when an Ec2 instance is launched into a specific subnet inside your VPC, a primarily elastic network interface (ENI) is provisioned into that subnet and is mapped to the physical hardware of that EC2 host for that AZ. And you can add multiple different ENIs to your ec2 instances.

So let's go back to storage and talk about how an EC2 instance can connect to an elastic block store, EBS. The way this works is that EBS lets you access volumes of persistent storage. Inside your VPC you have a data network set up for your ENIs, but you also have a storage network to connect to your EBS volumes. And EBS is an AZ resilient service, so you can have different EBS volumes running in different subnets for different EC2 instances but you cannot connect an EC2 instance to a EBS volume in a different AZ/subnet.

EXAM TIPS:

Understand the behaviors of Ec2 instances:

Your EC2 is running on a specific host, what happens if you restart your EC2 instance? Well it will stay with that same EC2 host, but if the instance is stopped and then started or if AWS stops the instance for maintenance etc on their end, the instance will be reassigned to another host in the same AZ. So EC2 instances live and remain inside one AZ, but you can migrate your EC2 instance by copying your EC2 instance and then creating a new EC2 instance in a new AZ and a great tool for that is snapshots and AMIs which we will dive deeper into both later. And usually EC2 hosts contain lots of different instances of the same type but different sizes, and we will learn all about instance types and sizes later, but lets quickly mention that you have two types of EC2 instances, burst and steady-state load and again we will cover more depth a bit later on.

EC2 instances
Let's talk about the different types of EC2 instances and a high level overview of which instance type would be the best choice for a particular scenario.

So let's start and look at what we get when we choose and launch an ec2 instance: we get a raw amount of CPU, Memory, Local Storage, and type of storage.

And we need to be aware of the performance for each instance type because with each instance type we will also get storage and network bandwidth, so we need to make sure we have enough bandwidth with the instance type we choose.

We also get resource rations when we choose a particular EC2 instance. And resource ratios are simply the amount of resource you get for each raw amount so for example, an instance that is more suitable to compute would give you more cpu and less memory than an instance more suited for memory which would give you more memory and less compute.

We also get additional features and capabilities with different instance types. Like GPU for graphic processing. Some instances come with GPU and some do not.

So again we come back to your account structure, your goals, your design, and so on. It is crucial to know your design so you know which instance type to choose,

Ec2 instances are group into 5 instance categories: and these categories help you select an instance type based on your particular workload

General Purpose: default steady state workloads, even resource ratios, and should be used as default unless you have specific requirements
Compute Optimize: and these instances are designed for high-performance computing like media processing, ML, gaming, scientific modeling, etc. these resource ration is usually. More CPU than memory and they provide access to high performance CPUs,
Memory Optimized: is great for processing large in memory data sets and database workloads, the resource ration is usually more memory than CPU
Accelerated Computing: is designed for specific requirements like hardware GPU, field programmable gate arrays, FPGAs)
Storage Optimized: is designed for application using data warehousing, analytics workloads, Elasticsearch sequential and random I/Os,
https://aws.amazon.com/ec2/instance-types/

https://ec2instances.info/

And then there are EC2 instance types for each of these instance categories.

Burstable instances: what happens here is that instances have normal CPU loads that are low and you have an allocation of burst credits that allow you to burst up and then return to the normal level. These are usually cheaper and a great option.

When you launch an EC2 instance, you will see the first option to choose is an AMI, an AMI is an Amazon Machine Image. We use AMIs to launch our instances. AMIs are regional so that is important to remember, each individual region has its own regional amis, and amis can only be used in the region it is in. AMIs also control permissions by default that are specific to your account, or you can set the AMI to be public, or add specific AWS accounts on to that AMI. You can also create an AMI from an existing EC2 instance to take the current configuration and make a template to make more instances. And this is great if you have an instance that has a certain OS or certain set of volumes attached, and configured to your exact business requirements, so we can create a template and create an AMI and use this template to create more instances specific to our requirements.

EXAM TIPS:

AMI = one region
AMI baking is the concept of creating an AMI from a configured instance
AMIs cannot be edited, you have to update the conf and then create a new AMI
AMIs can be copied between Regions
Default permissions are only for your AWS account but you can update the permissions
AMIs do contain EBS snapshot so you will be billed for that data stored
EC2 Storage
EC2 has local storage included with the AMI you choose and this storage is called direct attached or local attached storage. These are physical disks that are directly connected to a device, this storage is directly connected to the EC2 host and is called the Instance Store. And this type of storage is really fast bc it is attached to the hardware, but it does have a lot of issues: if the disk fails, if the hardware fail, if the instance moves between two different EC2 hosts, the storage can be lost.

Ee have an alternative type of storage we can use with our EC2 instances and that is Network Attached Storage, and this is where volumes are created and attached to the EC2 instance over the network, and AWS uses Elastic Block Store, EBS, for this. EBS is not as fast as Instance Store, but EBS is highly resilient and is separate from the instance hardware, so issues with the ec2 host will not impact EBS.

You may also hear the term ephemeral storage and this means storage that is temporary you cannot rely on this storage to be persistent. And the instance store is an example of ephemeral storage

And EBS is an example of Persistent Storage, which is permanent storage that lives on even if you delete your EC2 instance.

Now before we go much further I want to talk about the different categories of storage in AWS that we need to know for the exam.

Block storage which we were just talking about, this is EBS, it is a volume that is presented to the OS as a collection of blocks but there is no structure, just a collection of addressable blocks. These blocks can be mounted which means that file systems can be created on top of the block storage, and you can also boot off an EBS volume and this is why most EC2 instances use an EBS volume, block storage, as their boot volume and it is what stores the OS.

EXAM TIP: block storage does not have a structure, and is bootable. And is used if you want to use storage to boot it is block storage, if you want high performance storage inside the OSit will be block storage too.

File Storage has structure, and in AWS this is the Elastic File system (EFS). This is a ready made efile system with a structure. You can create folders and access your files, but you cannot boot from file storage bc you are just given access to a file system over the network but can be used for mounting but not for booting.

EXAM TIP: file storage has a structure, you can create folders, it can be mounted but not bootable. If you want to share a file system across multiple servers it will bd file storage,

Object Storage is a collection of objects and has no structure, it is not mountable or bootable, and can store anything, images, pics, vidoes, files, etc. The key is that object storage is flat and AWS uses S3 for its object storage. If you want access or to store virtually unlimited object data then it will be object storage. Object will be the keyword for object storage and S3.

So for the exam, know the differences between these storage options and their performance.

EBS volumes and snapshots
Let's pick up right where we left off and take a deeper dive into EBS and volumes. Remember EBS provides network storage for our EC2 instances, and we useEBS to create volumes in an AZ and these volumes can be attached to an instance in the same AZ. When we launch EC2 instances, in most cases we are using EBS volumes behind the scenes as our boot volume for that instance. EBS as a service, provides volumes which are allocated block storage and come in different sizes. Volumes are created in an AZ so you have to specify which AZ you want when you create a volume, it is HA and resilient bc the data in a volume replicated within that AZ.

EBS volumes also have different physical storage types to choose from: SSD or HDD and depending on which type you choose you will get varying levels of performance, so you can have more control over your IOPs and throughput.

EBS is billed per month based on a GB gigabyte and sometimes you are billed for a separate IOPs component.

Use EBS if you need HA and reliable persistent storage and if you need to create snapshots.

With EBS we can create 4 different types of volumes:

General Purpose SSD (gp2) and this is the default for most ec2 instances. Gp2 can only be attached to one ec2 instance at a time
Provisioned IOPs SSD (io1) also uses solid state storage, SSD. The biggest difference for provisioned IOPS and gp2, is an increase in your IOPs which is great for high performance low latency workloads that need higher throughputs. Io1 can be attached to multiple instances at the same time. If you have questions on your exam needing High IOPs choose io1.
Throughput Optimized HDD (st1) uses magnetic drives HDD, the t in st1 stands for throughput; you cannot boot on either HDD type of volume. The big difference between these two is the type of HDD types is the data needing storage, st1 is designed for frequently accessed throughput intensive workloads, like data warehousing.
Cold HDD (sc1) uses magnetic drives HDD based, the c in sc1 stands for cold so if you have any questions regarding needing cold storage, choose sc1. This type is designed for data that is less frequently accessed and cannot be used for a boot volume.
You can pick your volume type based on your performance needed.

So if you need maximum IOPs pick GP2 or io1 great for databases
Or if you need higher throughput pick st1 or sc1 great for log storage
Lets also cover EBS snapshots bc they are a really useful feature of EBS. Snapshots are a backup of our EBS volumes. Snapshots are incremental volume copies that are saved in an S3 bucket. The first snapshot is a full copy of your data on that volume, and then the next snapshots are only incremental copies so only data that has changed. And this can protect your data against any AZ issues because the data stored in s3 becomes Region resilient. So when we create EBS volumes, we can create a new volume or create a volume from a snapshot, and you can use snapshots to copy data to multiple AZ and also Regions.

As a SA, you have to be aware of snapshot performance for the real world and also your exam.

When you create a new EBS volume, there is no need to do any initialization, the full performance is immediately available, but if you restore a EBS volume from a snapshot it does take time to initialize, and if you attempt to read data that is not restored yet, it is very slow.

But you can force a read of all data immediately when you are completing a restore especially in production. Fast snapshot restore, FSR, makes the instance restore immediate. And you get 50 snaps per Region and FSR is an added cost.

And let's also cover EBS encryption: By default EBS volumes have no encryption, but EBS encryption does provide at rest encryption.

When you create an EBS volume initially it is not encrypted but you can choose to enable encryption, and when you do, EBS uses KMS and the customer master key. And we will cover AWS Key mgmt service in a later section. But when an encrypted volume is created, then KMS uses the CMK to create a data encryption key to encrypt the volume and can only be decrypted using KMS. If you make a snapshot of an EBS encrypted volume the same data encryption key is used for the snapshot, so the snapshot is encrypted and any new volumes made from these encrypted snapshots are also encrypted and share this key. But if you create a new EBS volume from scratch with encryption you will get a new data encryption key.

EXAM TIPS:

EBS volumes are created in AZ,
EBS is HA and resilient bc its data is replicated inside the AZ
With EBS volumes you can also create a snapshot to offer more HA
Usually with EBS you can only have one EBS volume attached to one EC2 instance at a time, but we now also have a multi attach option with Provisioned IOPs but you probably will not see that on your exam yet.
EBS has gigabyte per month cost
AWS accounts can be configured to encrypt EBS volumes by default
Each volume uses a unique data encryption key and snapshots and future volumes from your snapshot use the same dek
Once an EBS volume is encrypted you cannot select to un encrypted the volume
EC2 Instance Store
Let’s cover the second storage option for our EC2 instances, Instance Store.

EC2 has local storage included with the Amazon Machine Image (AMI) you choose, and this storage is called direct attached or local attached storage.

These are physical disks that are directly connected to a device. This storage is directly connected to the EC2 host and is called the Instance Store.  And this type of storage is really fast because it is attached to the hardware. But it does have a lot of issues:

If the disk fails,
If the hardware fails, or
If the instance moves between two different EC2 hosts, then
the storage can be lost.

So for the exam we need to be aware of the benefits and issues with instance store as well as when you would choose instance store in different scenarios.

Instance store is another block storage device, but ulike EBS, instance store is physically connected to one EC2 host. So that location for instance store actually gives it the highest storage performance because it is local to the EC2 host, and must be attached when the instance is created. You cannot attach an instance store volume after your launch an instance. And instance store volumes are included in the instance cost.

Remember that instance store is ephemeral storage, so they are temp storage, and as a SA you must consider this temp storage.

If an instance with instance store moves to a new EC2 host, that storage will be lost. If an instance was stopped and started, it will also lose the instance store volume. If you change the type of your EC2 instance you will also lose that storage. If you have a hardware failure, you will lose that data. And the number of instance store volumes and size you get with your instance is based on the type of instance you choose.

But the big benefit of instance store is that it gives you higher performance, because again, that instance store is local to the EC2 host, and it is so much more faster BUT it is only temp storage.

EXAM TIPS:

Instance store volumes are local to an EC2 host
You can only add instance store volumes to an instance at launch time
Data is lost if that instance is moved to another host, resized, restarted, or has hardware failures, and so on
Gives the highest data performance in AWS but comes with the risks of losing that temp data
Instance store volumes are included in the cost of the instance
So let’s cover scenarios when you would want to choose EBS volumes over Instance Store volumes and vice versa.

When to use EBS:

Remember EBS is HA and is reliable persistent storage. So if you need reliable and available data then choose EBS.
Also consider that EBS is separate from EC2, and can be attached to one instance, and then detached and attached to another instance. So if you need to have persistent storage that you can move to another instance choose EBS, and remember we can now multi attach volumes to more than one instance at a time, so EBS would be a choice for this scenario too.
With EBS we can create snapshots and create backups for our data, this cannot be done with instance store volumes.
Remember for the exam the cap for EBS volumes is under 80,000 IOPS anything more we need to choose instance store.
When to use instance store:

Instance store volumes are a great value and are included in the instance price, and the larger the instance size the more instance volumes you usually get.
BUT if you need high fast performance greater than 80,000 IOPs or more than 2,375 megabytes per second choose instance store.
Also great if you need temp storage, especially since it is included with your instance price.
Also great for stateless services that do not store any account or session info.
Elastic File System (EFS)
I want to cover Elastic File System (EFS) in our EC2 section we may dive deeper into EFS in the storage section.

EFS is really useful with most AWS infrastructures because it provides network based file systems that can be mounted within Linux EC2 instances. It can then be used by multiple EC2 instances at the same time. So it allows us to store data outside of the EC2 instance while providing scaling and self healing properties.

AWS EFS is the AWS version of NFS, network file system, version 4. And with EFS you create file systems and then those file systems can be mounted on EC2 (Linux) instances. EFS systems can be mounted on many EC2 instances and that data in that file system can be shared within the file system with all of the EC2 instances.

EFS is separate like EBS, but lives inside a VPC, and can be accessed via hybrid methods like VPN or DX which are hybrid network systems which we will cover in a later section.

EFS runs inside our VPC and we create file systems inside EFS. EFS is accessible because there are tagerts mounted inside each subnet in multiple AZs that adds HA, and your instance uses the mount targets to connect to EFS.

EXAM TIPS:

EFS is only for Linux instances
Two performance modes, General Purpose (GP) and Max I/O
GP is the default and is great for latency sensitive use cases: web servers, directories, and so on.
Max I/O can scale to higher levels of throughput with added latency, so there is a trade off, great for media processing
And for throughput we have two different throughput modes:

Bursting mode works like EBS GP2 volumes
Provisioned you can specify throughput separate from size and is more like provisioned IO1
EFS also has two storage classes:

Standard - default and used for data frequently accessed files
Infrequent Access - less expensive and for data that is not often needed
And you can also use lifecycle policies to move data between the two different storage classes

EC2 user data and bootstrap scripts
In an earlier lesson we talked about Amazon Machine Images (AMIs), metadata and bootstrap scripts, so I want to take a deeper dive and cover at a high level overview of EC2 metadata and bootstrap scripts and what we need to know for our exam.

Bootstrapping on an EC2 instance is the process of configuring an EC2 instance to perform automated installation and configuration steps before that instance is brought into an in-service state. And with an EC2 instance we accomplish this by passing a script via the user data part of the launch configuration. And this process will help an instance come into service when it is in a preconfigured state with configuration or software installed.

Bootstrapping is just a process that helps to build automation and to bring the instance in-service with a pre-configured state. This process performs software installation.

169.254.169.254/latest/user-data

169.254.169.254/latest/meta-data

These are internal IPs for AWS.  You can retrieve the IAM role from the metadata, but not the IAM policy along with the AMI ID, the instance ID, the host name, instance type and so on for our EC2 instance.

And for the exam you need to know the difference between metadata and user data:

Metadata is the info about the EC2 instance
User data is the launch script of the EC2 instance
And the user data is a piece of information that we can pass into an EC2 instance and it is executed by the instance's OS only once at launch time. So it only applies to initial launch.

Previously, we used an AMI with an eBS volume, but now the EC2 service provides user data to this instance, and will check the metadata IP for any user data.

EXAM TIPS:

User data is a simple block of data

User data is not secure, do not pass in creds in your user data

User data is limited in size, but you can pass in scripts to download that need data

User data can be modified when an instance is stopped

But only executed during initial launch

For the exam you may see a question asking how quickly can you bring an instance to in-service state, and for AWS AMIs is usually only minutes, but sometimes we need time to install apps, etc. so we need the time to be extended before an instance is in an in-service state.

And bootstrapping helps us install needed software before an instance progresses to the in service state much quicker

We can also bake this software into an AMI. AMI baking allows you to add the needed software to be added to the AMI before the instance is launched. So all the software is included in the AMI. And you can use both to provide optimal progression and with bootstrapping and the baked AMI you can get more flexibility with the configuration.

EC2 Bootstrapping is the process of configuring an EC2 instance to perform automated install along with configuration steps post launch before an instance is brought into service.

With EC2 this is accomplished by passing a script via the User Data part of the Meta-data service which is then executed by the EC2 Instance OS.

ENIs, IP addresses, and DNS
In this lesson I want to tie in some of the networking we mentioned earlier to get a better understanding of how your can interact with EC2 instances and connect to EC2 instances.

Architecture of an EC2 instance:

Each EC2 instance starts out with one elastic network interface (ENI), the primary ENI. You can also attach one or more secondary ENIs that can be in separate subnets but in the same AZ.

The ENIs are separate from the EC2 instance, not attached to the instance themselves. The primary ENI has the actual IP address for the EC2 instance, even though it appears that those IP addresses are attached to the instance, they are actually attached to the primary ENI for that instance.  When you launch an instance with security groups, the security groups are also attached to the primary ENIi not the instance itself.

The primary ENI has a Mac address and primary IPv4 private IP address. You can have zero or more secondary IP addresses for private and public IP addresses, and you can have 1 elastic IP Address (EIP) per private IP address. You can also have one or more IPv6 addresses, and you can have security groups.

Per ENI, you can enable or disable the source destination check, so if traffic does not match the address the traffic will be discarded and for NAT gateways this needs to be disabled.

You cannot detach the primary ENI, but you can detach other secondary ENIs and move them to other instances.

EC2 instances will also receive DNS addresses that can communicate with the private IP addresses inside your VPC.

EIPs: when we allocate an EIP we can associate the EIP with our primary ENI or our secondary ENI.  If we assign an EIP, then the instance will lose its public IPv4 address, if you remove the EIP then you get reassigned a new public IPv4 address.

EXAM TIPS:

SGs are attached to the ENI, not SGs
You can set up different SGs for multiple ENIs to have more secure connections
If you stop your instance, a new IPv4 address will be given to that instance. EIPs can solve this problem
Public DNS will resolve to your primary IP address inside your VPC, but the public DNS will resolve to the public IP from everywhere else.
EC2 Auto Scaling
Auto scaling groups (ASGs) are how we configure EC2 to scale automatically based on different criteria.  ASG uses launch templates or launch configurations.

A launch configuration:

ASG provides autoscaling for EC2 and can be used to implement a self-healing architecture, and they use the launch configuration to know what to provision.

ASG has three important values to remember:  minimum size, maximum size, and desired capacity. And an ASG provisions and terminates based on the number of instances they have currently and what the desired capacity is set too.

How it works:

If the desired capacity is more than the instances we have provisioned, then the ASG will launch new instances to match that desired capacity.
If the desired capacity is less than what is provisioned, then the asg will terminate instances to bring the actual number to match the desired capacity.
And we can use scaling policies based on metrics like CPU utilization.

If you have our launch configuration (min, max, and desired capacity) set to:

Minimum size: 1 instances

Desired capacity: 2 instances

Maximum size: 4 instances

Your launch configuration and auto scaling group will look and see you have:

1 instance for your min size, you will always have one running instance.
2 instances for your desired capacity, your ASG will take this launch configuration with a desired capacity of two instances and launch a new instance to match the 2 instances for your desired capacity.
4 instances for your max size, you could potentially have up to 4 running instances at a time depending on the metrics we assign.
So this can be done manually or we can add scaling policies to do this automatically. A scaling policy is rules that we define that adjust our values with our ASG. We also have scheduled scaling policies that are based on time-based adjustments. Dynamic scaling that are rules that react to a metric, and under dynamic scaling we have three sub policies:

Simple scaling, so it is a rule on a metric, so let's say our CPU utilization, memory, or disk I/O is greater than 50%, then add 1 instance. If the metric is lower than 50% remove one instance. This allows scaling in and out based on the metrics.
Stepped scaling defines more detailed rules. So add 1 instance if the metric tracks over 50% or add 3 if the metric is over 90%.
Target tracking is configured to define an ideal metric. Maybe you want your CPU utilization to stay around 40%. The point here is to maintain that level, and the ASG will adjust the size-in and out to maintain the value.
ASGs also have cool down periods which control how long to wait at the end of a scaling action before performing another action. You can use cool down periods to make sure scaling actions do not occur until a certain time has expired.

ASGs can also be configured to replace failed instances. The way it works is that it will see an instance has failed. The ASG will terminate the instance, and then launch a new instance to replace the failed instance. This self-healing feature is what we talked about earlier, in this situation the launch configuration would be a min of 1, max of 1, and desired capacity of 1.

ASGs can be used with load balancers. Load balancers use listeners that are configured and are pointed towards a group of EC2 instances in a target group. A target group is just a set of instances; you can link your ASG with this target group. And this is usually based on the load of the system to determine the scaling policy.

ASGs can use the load balancers for their health checks rather than the EC2 instances health checks.  Application load balancers have health checks that are a lot more defined and application-aware than the simple status checks of EC2.

EXAM TIPS:

ASGs are free at no costs, just the resources that the ASG creates.

ASGs use cool down periods and avoid rapid scaling

Use smaller instances bc it offers more granularity and has a cost savings over larger instances

ASGs and ALBs offer more elasticity because they are not connecting to the servers but to the load balancer, so they are abstracted from the instances and can use that capacity more smoothly.

ASGs define when and where to launch and the launch configuration defines what you want to launch

Launch configurations define what is launched:  what type of instance, what networking, what SGs, what AMIs, and so on.

ASG defines when and where to launch the instances, what subnet, what vpc, and so on.

Storage, Databases, and Migration
Storage intro
Earlier we covered requirements to consider when choosing a storage solution, but we also have to add into our considerations:

· Durability

· Availability

· Security

· Regulatory and governance requirements and

· Functional requirements

AWS storage solutions can meet different technical and price requirements. From a cost-optimization perspective, the lowest compute-related cost storage option is locally attached, ephemeral storage. This is storage included in the run rate for EC2 instances. The local processing nature of ephemeral storage isn’t for long- term, persistent data storage.

For more persistent storage, Amazon Elastic Block Store (Amazon EBS) enables EC2 instances to write to block-level devices that can be migrated to different instances. It also provides snapshot functionality to back up and migrate these volumes.

There are two storage types available for EC2 instances: non-persistent or ephemeral storage, which is appropriate for log files and non-critical data, and persistent storage for applications and workloads that require persistency.

Each option has pros and cons in terms of performance and costs. Ephemeral storage is included in the EC2 instance hourly rate. Amazon EBS comes at additional cost. You should consider these pros and cons per workload during your initial assessment, and then again after the workload has been running for a time. That way, you can see if you’re using the resources you’ve allocated and

make adjustments, if necessary. For example, among the Amazon EBS volume types, you could switch from Provisioned IOPS to GP2 instances if you find that your workload is more efficiently run on a “bursting” level of IOPS. AWS makes volume information available to customers through Trusted Advisor, which will highlight unattached Amazon EBS volumes and other important deployment information. In this case, with a proper archive strategy, deleting unattached Amazon EBS volumes will minimize storage costs.

Amazon S3
S3 is accessible from anywhere in the world with an internet connection and providing 99.999999999% durability. S3 has no limits on the amount of storage that can be used and provides mechanisms for customers to delete or archive (to Amazon Glacier) data no longer needed in quick-access storage. Using Amazon S3 lifecycle policies will enable you to migrate data from Amazon S3 to Amazon Glacier or delete it entirely. Amazon S3 also provides customers with storage classes8 with different levels of durability, availability, and pricing. These other classes can be useful when your storage mechanism does not require 99.999999999% durability.

https://www.youtube.com/watch?v=vFfY_-TL-pc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=6

Amazon Glacier
You can use Amazon Glacier to address your archiving requirements and improve your cost optimization. Amazon Glacier is, by design, cold storage. It should be used for data you need to retain, but do not need to frequently access. Although S3-to-Amazon Glacier migrations can be seamless, many small, frequent retrievals from Amazon Glacier will cause you to incur higher costs. For this reason, you should carefully consider a retrieval process.

https://d0.awsstatic.com/whitepapers/Cost_Optimization_with_AWS.pdf

Storage Gateway
Storage gwy is a service that allows us to connect your on premises data center and storage to AWS storage service. It allows us to migrate part or all of your storage platform to AWS or it supports extending your storage platform to AWS.

And we have three types of storage gwy:

File gateway: stores files as objects in S3 but has a local cache for your most recently accessed data onsite. Storage gwy is virtual appliance that you run on premises as a virtualization platform, so you can run it on VMware, esxi, ec2, and so on. You download and configure on your on premises location to talk to aWS over the internet. File gateway is a great option for Windows and is accessible using SMB and when you upload data with your storage gwy, that data is stored in S3.

Volume gateway: is configured the same way as file gateway. You configure and download the virtual machine image. However, when you access volume gateway, you are not accessing file shares, but volumes and these volumes are accessed over the protocol I-SCUZI which is generally used with SAN products, so it is network attached storage, and volume gwy works great with servers. You can also take snapshots from the volumes and create EBS volumes.

These are iscuzi presented volumes, and you cannot access the files indivudally without mounting the entire volume.

And you have two options for volume gateway:

Gateway stored volumes: which helps to store all your data on a volume gwy applicance itself and then snapshots are taken into aws stored on s3. This is used when you want your data on premises but snapshots backups in s3.

Gateway cache volume: which stores primary copy of your data in AWS and then downloads and caches frequently accessed data on the volume gateway itself.

Virtual Tape Library gateway: allows us to present a virtual tape library over ISCSI to any compatible backup software. This has a high admin overhead and is also costly, and should be stored off site. Allows us to present a virtual tape drive and it is stored in S3. Can be used to migrate your data into AWS over a period of time.

EXAM TIP: know each type of gateway and what purpose they would be used for.

FSx
Amazon FSx is a newer service and it is file server similar to EFS. Remember EFS is a shared file system for Linux and you can not use EFS for Windows. So AWS created FSx for Windows and it is a fully managed Windows file system share drive that supports the SMB protocol and Windows NTFS. It supports Active Directory integration and ACLs. It is build on SSD and is highly scalable  distributed file system for windows managed by AWS. It can scale up to 10 of GB per second and millions of IOPs and so on. It is highly availabe and can be configured for Mutli AZ. It can be accesed from your on premises, and your data is backed up daily to S3.

We also have another Amazon FSx for Lustre which is a type of parallel distributed file system for large scale computing. Lustre's name comes from Linux and cluster so that will help you remember it is for Linux instances and cluster is for the large scale computing.

EXAM TIP: Lustre is great for ML and High Performance Computing (HPC), you will probably see HPC on your exam a few times, Lustre has sub-milisecond latency.

Lustre is also great file system to perform video processing, financial modeling, design automation whatever needs a high-level of distribution. It seamlessly integrates with S3 and you can read your s3 buckets as a file system using fFSx Lustre and write computes back to s3.

Databases
RDS
RDS stands for relational database service, and RDS is considered a Database-as-a-service DBaaS.  RDS is an AWS service that provides managed database instances, and with RDS you are paying for and consuming a db server that we have access to.  AWS handles the management, and we get access to a managed db instance and this provides lots of benefits, and performance enhancements. We do not have to manage the physical hardware, the OS, and so on and RDS supports MySQL, MariaDB, PostgreSQL, Oracle, and Microsoft SQL Server, andAmazon Aurora. So you can pick which db works with your application requirements.

RDS databases come in different types, sizes, and families just like EC2 instances. RDS instances can be in one AZ or in multiple AZs.  For an RDS instance you allocate storage for that instance to use, so it is dedicated storage for that db instance.  And access to and for your db instances are controlled through SGs. RDS instances in a single AZ can be vulnerable to a failure in that single AZ because the instance and the storage are in a single AZ.

Multi AZ allocates secondary hardware in a different AZ. This second db instance is called the standy by replica instance. RDS uses synchronous replication from the primary and the standby instance.

With RDS you access your db instance by its CNAME and that CNAME points to the primary instance only, so you have no access to your secondary instance. You only have the single endpoint address pointing to the primary replica, you cannot use your standby instance for extra capacity etc, it only accepts synchronous replication from the primary instance.

The writes are committed to the primary instance replication to the standby at the same time. Now if for any reason our primary instance fails, RDS will detect this and change the CNAME to point to the standby instance. And this may add a brief interruption, but this failover provides HA and it automatic.

RDS read replicas provide two main benefits, performance benefits and availability benefits.

A read replica is a read only replica of your RDS db instance, and you can read replicas for read operations, and data is replicated asynchronously.  And asynchronous replication it is written fully to the primary instance first, and then it is replicated to the read replica, so there can be seconds of lag depending on your network conditions etc.  Synchronous replication is completed in Multi AZs and the data is written to the primary instance and replicated to the standby read replica at the same time.  So on the exam if you see asynchronous think read replicas and synchronous replication would be the choice for any question with a multi AZ env/scenario. Read replicas can be in the same region or different aws regions, if different aws regions it is cross region read replica. Read replicas are important bc they provide performance improvements.

If you have 5 read replicas per db instance with RDS, each of those read replicas provide and allow you to scale out read capacity for a db, so your application can perform reads against the read replica and not against the primary db instance. Then you can use the primary for writes only. You can create read replicas of read replicas but this adds lag and this lag can start to be a consistency problem. Read replicas also provide global improvements bc it scales reads; it is great for availability improvements, and offer global resilience bc you deploy read replicas all over the world.

We can use snapshots and backups to improve RPO, recovery point objective, and read replicas offer near zero RPO. This is done asynchronously from our db instance and if our primary fails then we can promote our read replica to be our new primary instance within minutes. This only works for failures bc read replicas will replicated corrupted data, and then at that point you could not use this as a failover, you would have to use a snapshot before the corruption.

RDS backups, snapshots, and restores

It is important to understand these RDS features bc not only will you see exam questions but you also need to make sure your data is secure, and you also need to understand these features for DR.

From our AWS Fundamentals we talked about DR and we learned about RTO, recovery time objective, and RPO recovery point objective. Remember that RTO is your recovery time objective, so it is the time between a failure and when you system is back online, and again lower rto is usually more expensive bc you need more resources

RPO is the time between when the last working back occurred and when the failure occurred, and it is the maximum amount of data you are prepared to lose, and the lower your rpo usually means more expensive, bc you need more backups and more resources

So with backups it is important to know your RTO and RPO requirements. For RDS we have two types of backups: automated backups and manual snapshots. S3 stores the backups/snapshots in S3 managed buckets. This adds to our backups, region resilience because remember S3 replicates our data across at least three AZs in a region.

Snapshots are manual snapshots that you take of your db instance, and again stored inside S3 similar to EBS snapshots. The first is a full copy of the data and then are incremental, and there is a brief interruption during your snapshots, and with single AZ there is impact but again on multi AZ there is no interference bc the snapshot is taken on the secondary db instance. It is important to remember that you must go in and delete your snapshots, you have to remember to delete those snapshots and if you delete your RDS instance or you will continue to pay for that storage. You can take a snapshot of your instance before you terminate your instance for good.

Automated backups are also snapshots and you choose the time of that backup window, the first is a full copy and then after they are incrementals. These are not retained and are automatically cleaned up and you can save these for 0 to 35 days before they are automatically deleted. You choose the retention period. DB transaction logs are written to S3 every 5 minutes so your db can be restored to a specific point in time.

As far as billing, you are billed for your RDS instance, an hourly rate for the compute and amount of storage that you allocate to your instance.  So like EBS you are billed on the amount of storage you allocate, not what you use.  It is a gigabyte per month metric for billing.

EXAM TIP:

Multi AZ

This feature is not available with the free tier bc you are using extra resources

RDS multi AZ does not scale your reads, it cannot be accessed directly and the standby provides not added performance, it is only good for HA.

Multi AZ is in the same region only - cannot be used across regions

Backups can be taken from your standby instance so backups have no performance impact or interruptions on your primary instance - backups in a single az will cause performance issues

Remember asynchronous is Read Replcias and they are for read scaling

Synchronous equals multi AZ for HA

RDS handles restores by creating a new RDS instance, with a new db instance endpoint address, so your application will need to be updated

When you restore a manual snapshot, you restore that db to a single point in time, and this can influence your rpo

Automated backups have transaction logs recorded are every 5 minutes

Backups are restored from the closest snapshot and transaction logs are replayed to bring the db to the desired point in time

Restoring snapshots is not fast, it can take a long time and is not always great for DR, bc that restore time influences your RTO, what will help is read replicas

But if you have data corruption you should use restore bc corruptions will be replicated to RR.

https://www.youtube.com/watch?v=igRfulrrYCo&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=7

Aurora
Aurora is a relational db and part of RDS, but it does have quite a few differences and improvements over RDS.

First the Aurora architecture is very different from RDS, Aurora uses the base architecture of a cluster.  And it compatible with MySQL and PostgreSQL engines. It is a cluster made up of a single primary instance and then zero or more read replicas. This may seem the same as RDS but Aurora read replicas can provide the benefits of reads and also the benefits of multi AZ. So they can be used to improve availability and read operations on your cluster.

Second, Aurora storage is different from RDS because Aurora does not use the local storage for the compute, it actually uses a shared cluster volume, which provides faster provisioning, improved availability and better performance.

You can have up to 15 read replicas with Aurora and each can be a failover choice. And since Aurora read replicas do not have the local storage like RDS, Aurora read replica can be added and removed without requiring storage provisioning, so it improves our speed and efficiency of our replica changes in the cluster. Each instance in your cluster receives an endpoint, remember for RDS only the primary db instance had an endpoint, but with Aurora each reader also gets an endpoint along with the primary cluster endpoints for writes. And you can create custom endpoints too.

Billing for this storage is based on what storage you consume,

Aurora cannot be used in the free tier

Compute is charged hourly and you also have a storage cost as well that is billed in GB per month consumed and your backups are included at 100% of your storage consumption

and with aurora provisioned single master we can have aurora serverless and aurora global dbs, and we will cover those in just a minuted

Backups in Aurora work the same as they do in RDS

Resotres create a new cluster

Aurora also offers BackTrack which must be enabled but allows you to roll back your database to a previous point in time, so no application configuration updates are needed, it is simply rewinded to that point in time.

Aurora also offers fast clones by referencing the original storage and only stores the differences between the two dbs.  Clone dbs only uses a small amount of data, stores data in the original after the clone and the clone itself.  Only the changes are stored bw the source databases and the clone.

Failovers, well when the cluster realizes there is a failure, then the primary failover to one of the read replicas, and this can take some time.

In a single master mode for Aurora you can have multiple endpoints. There is a cluster endpoint that is used for writes and we have up to 15 reader endpoints that are used to load balance the reads.  And with this single master the failover to a read replica can take a bit of time, because the reader has to be promoted to a read and writer.

But with multi master all of the instances in your cluster are capable of reads and writes, so the failover is much quicker. The same architecture exists, the difference is there is not a cluster endpoint to use, and there is no load balancer the application connects to one or both of the writer instances. When a multi master receives a write, the data received is sent to the storage cluster across all 6 storage nodes. With multi master the writers can also add that data to their in memory cache. For multi master failover, you have two writer instances, so if a writer fails then Aurora will simply send the requests to the one writer instance that is still working.  So it is much smoother and much quicker than in a single master architecture.

Aurora Serverless is a service of Aurora and provides a version of the aurora db product where you do not have to provision or manage the db instances. Aurora serverless works a bit differently architecturally. Aurora serverless provides the same shared cluster storage so you get again 6 copies of your data across three AZs. But we do not provision our cluster the same way, with Aurora serverless we use ACU which is aurora capacity units. The Aurora ACUs provide a certain amount of compute and a corresponding amount of memory. So for an Aurora serverless cluster we can choose a min ACU and a max ACU and then your Aurora serverless cluster will scale between that min and max value and will add and remove the capacity in your cluster based on the load. A really cool feature of Aurora serverless is the ACU can even go down to 0 and then can be paused after a period of inactivity so this is a great cost savings, because when your cluster is paused you are only paying for the storage that you are using. Billing for Aurora is based on the resources you use and are billed on a per second basis. You probably will not see Aurora serverless on your exam but I did want to cover it in case you do see questions on your exam.

Aurora Global dbs allow you to create global level replications and up to 5 secondary replications per region. It probably will not be featured on your exam, but again lets cover it at a high level. With Aurora global dbs, the primary region of a global db is very similar to aurora provisioned: you have one read and write instance and then up to 15 read replicas, but with Aurora global dbs, the second region's cluster is read only. You can have 16 RRs but again those are only read replicas, you do not have a writer instance. And replication is typically one second replication to the secondary regions which is sooooo fast and this replication occurs at the storage level so there is no impact on the db performance bc it is replicated at the storage layer.. And replication is only one way. Aurora global dbs are great for DR, and you can failover your primary cluster to your secondary clusters just like with provisioned Aurora. Aurora global dbs offer low latency and performance improvements if you have international users or customers.

DynamoDB (DDB)
DDB is a Nosql database as service product, and it is a public service and sits in the AWS Public zone. From the VPC section, we learned that we can use endpoints to access services inside the AWS public zone. So we can use the public internet to access DDB, or access it from inside a VPC with an internet gateway, or we can use a VPC gateway endpoint.

AWS manages DDB for us, we do not need to manage any servers or infrastructure and DDB can handle simple key value data or structure data. DDB also supports scaling options: using provisioned capacity with manual controls or use on-demand mode which handles scaling for us. DDB is highly resilient across multiple AZs in a region or you can configure a global table to add global resilience but this will be an extra cost.

DDB’s data is replicated across multiple storage nodes by default, and it is fast and backed by SSD. DDB also handles our backups, allows for point in time recovery, encryption at rest, and can support event driven integration to take actions if your table changes. Well, what is a table. A table is the base entity in DDB. A table is a group of items which all share a primary key, and items in that table is how you manage that data in the table. An item is like a row  and tables can have lots of items, there is no limit.

When you create a DDB table you have to pick a primary key and there are two types:

Simple (Partition) Key or Composite Key

The Simple Key is just the partition key (PK)
The composite key is a combination of the partition key and the Sort key (SK)
Every item in the table has to have the same primary key and it has to have a unique value for that primary key, but if the primary key is a composite key then the combination of the two parts the PK and the SK need to be unique in the table. And then your other items besides the primary key can have different attributes and this data can have all, a mixture, or completely different attributes. All items can be up to 400 kilobytes in size.

DDB can be configured with Provisioned or On-Demand capacity, and adding capacity means adding more performance, more speed, and so on.

On-Demand Capacity is handled for us, we do not have to set explicit values, we just pay for operations on our table, so cost per operation.
Provisioned Capacity is explicitly set on each table: write capacity units and read capacity units.
1 WCU = 1 KB per sec you can write one kilobyte of data per second to that table

1 RCU = 4 KB per second you can read 4 kilobytes of data per second from that table

DDB backups offer two types:

On demand and these are similar to manual RDS snapshots. DDB on demand backups are a full snapshot of our table that is stored until we delete that backup. It is stored in the same region or can be stored cross-region. It is a manual process, and you can adjust encryption and remember for cost savings to remove and delete the backups when they are n olonger needed.
DDB also offers point in time recovery and this type of backup can be enabled per table, and when enabled it is a continuous stream of backups of all changes to your table over a 35 day period. And you can restore anytime from any one second interval within that 35 day window if backups.
We can access DDB via the console, CLI, and API. Billing is based on the set RCUs, WCUs, and the storage plus any features you enable. You can use reserved capacity for an added cost savings but you do have the longer term commitment.

So remember we can choose between two different capacity modes when we create a table: on demand and provisioned. And you can actually switch between these two modes if needed.

On demand is designed for when you have an unknown design or unpredictable load and remember we do not have to explicitly set our capacity settings but this is more expensive than using provisioned capacity, you pay a price per million read or write units.
With Provisioned capacity you set a capacity value for our reads and writes on each table and those are rcus and wrus
And every operation on your DDB table will consume at least 1 RCU and 1 WCU

Capacity is rounded up, so even if you consume less than 1KB, it will round up to 1 KB

EXAM TIP:

1 WCU = 1 KB per sec you can write one kilobyte of data per second to that table

1 RCU = 4 KB per second you can read 1 block of data up to 4 kilobyte of data per second from that table

And each table has an RCU and WCU burst pool that equals 500 seconds of the read and write capacity units of our table, but this pool is also used by other table tasks, so try to reserve this pool when it is needed only.

EXAM TIP:

We can perform lots of types of operations on our ddb table but the two you will probably see on your exam are query and scan.

A Query is a way to retrieve data from DDB, and we use a partition key value to start this query, so we specify a single value for our partition key, and that will return an item or items. It is always more efficient to pull as much data as possible in one query, so we do not have multiple reads and waste our RCUs. We can also filter this down by adding a sort key value or a range of sort key values. So a subset of sort key values, we are billed for the returned data. And filters are charged for the entire size of the items, so it is best practice to minimize the size of your items.
And to perform more flexible operations we can use scan, however, it is not efficient for getting your data, but it is flexible. So you can choose a specific attribute or filter and those will be applied to our scan. And the scan moves through your table and consumes the capacity of each item in the table, so the entire table is consumed, but it will give you control on what data is selected. However, it does access every item so the whole table is consumed. It does not return items that do not match the attributes selected and added or the filter selected and add but it consumes the entire capacity of that table.
DDB also has two different consistently read modes. Consistency is the process of when new data is written to the db and then read, is that data the same as the most recent update or is it eventually the same.

Strongly consistent writes and Eventually consistent writes. Strongly consistent writes are more costly and do not scale well. Eventually consistency is easier to implement and scales much easier.

In DDB every piece of data is replicated in separate AZs, and each storage node in the 3 different AZs and one of these nodes is the leader storage node. So when our items are replicated across the storage nodes, and one of our items is updated, it is then written to our DDB table. Writes are directed to the leader node with the updated item, then the leader node is consistent because it has the updated data. Then the leader node will start replicating the updated item to the other storage nodes to also make them consistent.

With ddb we also have eventually consistent reads and strongly consistent reads:

Strongly consistent reads is 1 RCU = 4KB always use the leader nodes which is the first node updated.
Eventually cons reads are cheaper and you can read twice the amount of data on the same RCU.
So if we use eventually consistency then DDB directs us to one of the three storage nodes for our table, and the storage nodes usually have the same data but sometimes the writes are not updated and you could get older not updated data, so you will not always get the latest data but you get a cheaper price, so it is half the price of Strongly consistent reads but the data may be old.  It is not often but it can happen. But some applications cannot tolerate the eventually consistent reads, like stock apps, medical records apps, and so on.

How to determine our values for our capacity for our DDB table:

What if we need to store 10 items in our table every second. And the average size is 2KB

We first need to know the average size of our item and how many items per second will be written. If you have questions based on minutes, remember to switch the minutes to seconds bc that is whole we calculate our capacity.

So to calculate WCU per item = we take the item size 2.5KB) and divide it by 1KB = 2.5and round that up = 3

Then we multiple by the average number of items (10) per second (3) to get our calculations = 30 WCUs

Let's also look at read calculations, so to calculate the RCU per item =

So let's use the same example, so we need to retrieve

10 items per second and the average size = 2.5K

So we take the item size and divide it by 4 KB and then round up that number.

(item size/4KB) then round up .   (3/4KB)=.75, so rounding = 1

Multiply by average read op per second (10)=10 so 10*1=10

Strongly consistent  RCU = 10

But for eventual consistent read we divide the RCU value and divide it by 2

10/2=5 5 RCUs will be required

**These calculations will feature heavily in your Certified Developers Associate exam but you may get a question on your SA exam. But it is really good to have this understanding, but for the exam remember the size of an RCU and WCU for the associate exam.

Let's wrap up DDB and talk about DDB streams and triggers.  They can be valuable to cost optimize your DDB table. A DBB stream is an ordered list of changes inside your DDB table, so each change Is recorded in order to this DDB stream and a DDB stream is a 24 hour window of all changes, and can use Kinesis streams. You do have to enable streams on each DDB table, and you can configure your stream to have different views: keys_only, new_image, old_image and new_and_old_image. Streams can be used with db triggers so it allows you to take actions when changes in your data occur, and we can implement this in a serverless way. And this saves money because you do not have to poll your dbs and only consume the minimum amount of capacity required.

EXAM TIP:

Know that you can use DDB streams and Lambda to create triggers and can then take action.

If you see questions asking for NoSQL then the answer is probably DDB, NoSQL is a keyword.

If you see relational db in the question then it is not going to be DDB, DDB is a non relational db.

If you see key value in your exam question then DDB could be the answer.

If you see any questions with SQL or the structured query language then DDB is probably no the correct answer.

https://www.youtube.com/watch?v=skr_raPPvTc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=26

OpenSearch
Elasticsearch (recently changed to OpenSearch) not sure which name will appear on the exam

Amazon Elasticsearch Service is a fully managed service that enables you to search, analyze, and visualize your log data cost-effectively, at petabyte-scale.

Elasticsearch clusters are challenging to set up, scale, and manage. As a fully managed service, Amazon Elasticsearch Service manages the setup, deployment, configuration, patching, and monitoring of your Elasticsearch clusters for you, so you can spend less time managing your clusters and more time building your applications. With a few clicks in the AWS console, you can create highly scalable, secure, and available Elasticsearch clusters. Amazon Elasticsearch Service offers open source Elasticsearch APIs, managed Kibana, integration with Logstash and other AWS services, and SQL querying, so you can continue to use your existing tools and code.

Elasticsearch, allows us to search any field in a db, even partial matches.  ES allows you to build a cluster of instances, and it integrates with kinesis firehose, IOT, and CW logs, for data ingestions. It works great with DDB, but with DDB you can only find. Data with exact matches on the primary key or indexes, but with  ES we can search any field and partial matches too.

AWS secures ES using Cognito, IAM, KMS, and SSL and multi AZ clustering

EXAM TIPS:

And ES works great with Kibana for visualization

Cost is pay per provisioned node.

ES allows us to search any field.  It is great for searching and indexing.

RedShift
Redshift is a petabyte scale data warehousing solution form AWS, it is a column based db engine for analytical workloads. Most RDS dbs are used for OLTP, online transaction processing, but Redshift is designed for OLAP, which is an online analytical processing, and it is not the type of db where you update individual records, it is used for data warehousing analytics, and everything is stored in columns.  And column based dbs are great at queries because all data is in columns. Row based dbs are great for transaction type processing and column based dbs for analytics. Redshift is based on PostgreSQL but is an OLAP. Redshift is NOT used for OLTP. Redshift uses a cluster architecture and unloads and uploads data to S3. It can also accept data from DDB, Database Migration Service (DMS), other dbs, and Kinesis too. And to go along with S3 we can use Redshift Spectrum to perform queries directly against S3. This is not like Athena, with Redshift Spectrum you must have a Redshift cluster, but you do not need to load the data into Redshift: you can simply queries directly from S3. Athena is serverless so there is not an instance to provision.

Redshift also has point in time backups that are stored to S3, and snapshots are incremental and occur every 8 hours, every 5 GB, or on a schedule. And you can select a retention period.    Only the data that has changed is saved, and we can use the snapshots to restore to a new cluster. Redshift can also be used with DR, we can configure Redshift to automatically copy snapshots of our cluster to another AWS region. As far as cost, we pay for what we provision (so the instances we provision), per node provisioned. Also for cost optimization all manual snapshots are retained in S3 until deleted.

EXAM TIP:

Know that Redshift is a data warehouse used for analytical and summarization transactions, and can scale to almost any workload needed and is a petabyte scale db.

Elasticache
Elasticache, which is a managed in memory cache for performance improvements for reads.  It supports two different popular caching engines: redis and memcacheD. So if you see a question with memcached or Redis your answer is probably EC. EC is designed to store reads and deliver those results from in memory caching and improves performance, so instead of consulting the db each time for reads, you can cache results and then deliver those results quicker. EC can also be used to store user session states. And we mentioned sessions in the fundamentals section, but you can store the users session states using EC. And EC can be used as a performance enhancing tool or used with fault tolerant architecture.

You should not see too many questions on your exam but may see one or two.

DDB Accelerator (DAX)
Lets talk about DAX too because EC used to be used with DDB, but AWS created DAX to be used specifically with DDB. DAX is the DDB accelerator. As we learned earlier, DDB, is designed to be a low maintenance and high performing db that provides access to data in milliseconds, but we do have edge locations that need this data faster like microseconds, and also for high read sessions, and DAX provides an in memory cache for DDB.

DAX runs inside your VPC and uses a cluster architecture so we can have one or more nodes, and applications use a DAX client installed on the same resources as the app itself. So when items are read from DDB, the items are returned to the application, but also stored in DAX. And if that items is read again it is returned using DAX without using DDB. And that is called a cache hit, if it is not in DAX, then it gets pulled from DDB and is stored in DAX and is then returned to the application. And that is known as a DAX miss.

DAX is designed for latency sensitive and high read workloads

DAX also has two distinct caches: the item cache and the query cache.

The item cache is made up of results from GetItem and BatchItem and comes with a 5 minute default TTL, the query cache stores results of Query and Scan operations and caches the results based on parameters specified.

You can also use Elasticache/OpenSearch for DDB also, but DAX was specifically designed to work with DDB so it is the preferred in memory cache for DDB.

EXAM TIPS:

So you may see a question asking what is the best caching product to use with DDB and the answer is DAX.  Dax is NOT great for applications that need strongly consistent reads. Dax is more for eventually consistent reads.


High Availability and Scalability
Load balancers are used to achieve high availability, fault tolerance, and scaling. So let’s cover the essentials of load balancers.

So what is a LB? Load balancing is a method used to distribute incoming connections across a group of servers or services. And incoming connections are made to the LB, which then distributes them to the servers or services.

In AWS we have four choices for LBs, Classic (CLB), Application (ALB), Network (NLB), and the Gateway Load Balancer. And these four make up a family of elastic load balancers (ELBs) and they are great to pair with auto scaling groups to enhance the high availability, fault tolerance, and scalability of an application. For the exam know that LBs have listeners that listen for traffic protocols and ports. In AWS HTTP listens on port 80 and HTTPs listens on port 443 from users, and then behind the LB we have the app server/s. When a user connects to the LB, then the LB takes those requests and distributes those requests between the application servers.

The architecture is that connections are made from the client to the LB, and then the LB decides which instance to use. Then the LB makes a connection with the backend instance and sends your request to that instance or brokers that connection, but if you click on another link you might be switched to a different instance.

So there are two separate connections, one from the user's client to the LB and then another connection from the LB to the particular application server. And these two connections are called the listener connection and the backend connection.

When you create a LB you are creating one entity, one LB, but it actually creates an ELB node.  For HA, a LB node is placed in each AZ that a LB uses. And the ELB gets a DNS record that automatically points to the ELB nodes, and the connections are split between the nodes. For the exam know, you can enable cross zone LBing to allow each node to distribute traffic to all instances. And this is enabled by default.

LBs also run health checks against all servers, if one fails, then the LB will stop sending requests to that failed server.

LBs are great for HA, scalable and fault tolerant architectures. If you deploy an application rather than point the application to one or more instances, specifically you can simply point to a LB that has two or 50 attached instances.  That helps scale and also adds HA if an instance fails then the LB will send that connection to another instance.

Exam tips:

Clients connect to the load balancer's listener configuration, and then the LB connects on your behalf to one or more servers for the application.

ALB - Application Load Balancer
AWS started off with one type of load balancer which was an ELB, elastic load balancer. However, it did not provide a lot of features, so AWS added more features and created an ALB and then even more features were added and AWS released the NLB.

So the legacy LB for AWS, the ELB, is actually the CLB classic load balancer and with the ALB and NLB makes up the family of three products known as ELB. There is a newer load balancer that was added too, the Gateway Load Balacner.

Exam tips:

The ALB is known as a layer 7 LB from the OSI model, and at layer 7 this means that the ALB can inspect data that is passed through it and can understand the application layer, HTTP and HTTPS. The ALB can then take actions based on things in that proctol like paths, headers, and hosts.  And all AWS LBs are scablabe and HA.

And like we learned in the last lesson, the ALB is actually individual ALB nodes running in each AZ that is configured with your ALB.

So we did not mention this is the last lesson but LBs can be internet facing or internal, and the difference here is that internet facing have public IP addresses and internal LBs have private IP addresses. An internet facing LB is designed to be connected from the internet and LB those connections against the target instances, and internal LBs  are not accessible from the internet and are used to LB inside the VPC or between tier of a multi tier applications.

And again it listens from the outside and sends that traffic to targets or target groups. ALBs are billed at an hourly rate and an addition of the loadbased on the load placed on your ALB.

And remember ALB can also perform health checks across all its targets / instances. If one instance fails, then the target state for that instance will move to unhealthy and the ALB will no longer send requests to that instance.

So when you design the ALB architecture, you will see that ALBs have different services they can send requests to that are called targets .

So targets can be EC2 instances, containers in ECS, lambda functions, and so on. Targets are then grouped into target groups, and individual targets can be members of multiple target groups. And ALBs send requests to these target groups. So with ALBs you define listeners and rules that can be host rules or path rules.

NLB - Network Load Balancer
As we mentioned in the last lesson, ALB is recommended because it supports the functionality of the CLB and also supports layer seven protocol, HTTP and HTTPs, but what do we do if we need to load balance protocol that is not HTTP and HTTPS? We need the packets to remain untouched, so we need to support a protocol that is not web or secure web. It needs to be highly performant and put the packets through to the destination without any modification, well this is when we would use NLB and they operate at layer 4 of the OSI model. NLB and they do not touch that data in packert above layer 4. We can support other protocols as long as it utilizes TCP or UDP.

Exam tips:

NLB has advantages over ALBs.

NLB does not need to worry about the upper layer protocol, it is much faster.

It is able to handle high end workloads and scale to millions of requests per second.

We can allocate static IP addresses so it is easier to integrate with security and firewall products.

NBL supports routing requests on multiple apps on a single ec2 instance

And supports the use of containerize apps.

ALB is great for high end layer 7 protocol support
NLB supports any other protocols and can handle millions of requests.
So if you get a question asking which ELB can handle millions of requests then NLB should be your answer.

CloudFront
You should see CloudFront (CF) feature heavy on your certification exam, so let’s cover everything you need to know.

CF is the content delivery network in AWS. It is a global object cache, content delivery network or CDN, so instead of your global customers connecting directly with your application or content server, with CF, your content is cached in global locations that are as close to our customers as possible.

So if the content is cached in CF locations then it is directly delivered to your customers,if not then it is fetched, cached and then delivered to your customer.

So CF brings lower latency for your customers and higher throughput, so faster page loads and interactions with the apps.

CF can handle both static and dynamic content.

So lets cover CF concepts before we see the CF architecture bc it is important to understand terms and know what they mean as a fundamentals but also we need to know these for the exam and for real world too

Origin is the original location of your content. This can be an s3 bucket or an ALB or anything on the internet as long as CF can access it.

Distribution is the unit of configuration in CF, so we have to configure a distribution and then this distribution is deployed out to the network.

Edge locations are the global infrastructure where your content is cached. There are more edge locations than regions and AWS currently has over 200 edge locations throughout the world.

And we also have regional edge cache, and these are larger and hold more caches than the edge locations. There are not as many spread throughout the world.

CF integrates with the AWS Certificate Manager(ACM), so you can use CloudFront to add HTTPs capability to your statically hosted website running on our S3 bucket. AWS Certificate Manager is a product that lets us manage and deploy public and private certificates to use with AWS services. Certificates allow HTTP sites to handle encryption and allow it to prove its identity. HTTP is a simple and insecure protocol, so new server identity authentication or transport encryption was built into HTTP, but security vulnerabilities became an issue, so HTTPs was designed to address these security vulnerabilities. HTTPs uses SSL/TLS secure tunnel. It adds a layer of encryption and data is encrypted during transit and allows identities to authenticate, with the certificates we prove our identity and are trusted as a signed authority

So ACM creates and renews and deployed certificates to AWS supported services, like CF and ALBs, usually managed AWS services are supported with ACM.  But not EC2.

And if we use a certificate with CF or an ALB, then that communication from our users and the edge locations are encrypted, and the edge locations will communicate with the origin using the protocol configured. BUT if your CF distribution is set to communicate between the edge locations and the origin using HTTPs you need a trusted signed certificate.

CF is only for download style operations only but does support uploading content with five additional http methods, POST, PUT, DELETE, OPTION, AND PATCH. But when content is uploaded CF sends the upload request back to the origin; CF does not cache writes. You may see a question around this on your exam. CF does not handle any writes caching.

And CF can be configured to be private, so if you are using a private CF distribution then you need to prevent direct access to your bucket bc making CF dist private will only affects access via the edge locations, so users can access the bucket directly using the buckets dns then the CF restrictions will not apply, so make sure you removed direct access for your bucket.

What if we want to make sure that users cannot directly connect to our s3 bucket, and we want customers to use CF and the edge location. We can create an OAI and this is an Origin Access Identity. Once created we can associate this identity with a CF distribution, and this will give our edge locations this OIA ID. We can then add a bucket policy to allow the OAI, and remove any other explicit allowances for the bucket policy, remember only one bucket policy can be attached to a bucket at a time. So once this is completed all access from the edge location will be the OAI ID from our edge locations and S3 will know this is from the OIA /edge locations and access will be allowed but any other access will be denied. OIA can be used on CF distribution and buckets at the same time but it is best practice to create an OAI for each distribution.

Global Accelerator
Let’s discuss the global accelerator which adds lower latency for users. We just covered CF but what is the AWS Global Accelerator? We need to know both for the certification exam.

The AWS Global Accelerator uses the AWS global network to route the application and instead of using the public internet. And it is a service that is used to improve the availability and the performance for your users. The GA uses the public internet until we hit that edge location and then uses the AWS global network. So our traffic is sent to the closest edge locations through the private AWS network but without the AWS GA your traffic/packets will take different hops.

And the AWS GA works with elastic IP addresses, EC2 instances, ALBs, NLBs, and GA can either be public or private. It offers intelligent routing to lowest latency and fastest regional failover. Uses health checks to perform health checks on your application, and is also great for DR. With AWS Shield which we will cover in an upcoming lesson we can use AWS GA and AWS Shield to offer DDoS protection.

So what is the difference between CF and GA because they both use the AWS global network and the edge locations. Both also integrate AWS Shield for DDoS protection.

But here are the differences:

CF will improve content for cache content both static and dynamic content and content is served from the edge locations most of the time.

GA improves the performance for applications over TCP and UDP because the packets are being proxied from the edge locations to the apps running in one or more regions. So all requests are making it to the edge and there is no caching available. GA is great for HTTP use cases that need a static IP, or need fast regional failover.

Route 53
Let’s do a high-level overview of Route 53. So what is Route 53? Well, it is AWS's managed DNS (Domain Name System) product and it essentially helps us with two things: first we can register domain and second Route 53 can host zones on managed nameservers.

Route 53 is a global service with one single database and it is replicated between regions - making it a globally resilient service - meaning that it can tolerate the failover of one or more regions and continue to operate. It is a huge hierarchical database

DNS is a service used to help discover other services on the internet.  And it translates addresses from the language that computers understand to the language that humans understand and then back again. So if we want to go to amazon.comwe type in amazon.com, but computers use IP addresses, so DNS translates our words into IP addresses and then finds that location; it then sends that location back to us and translates the IP address back to words that we can understand.

The two main functions of Route 53 that we mentioned: Registering Domains and Hosting Zones.

Route 53 can register domains and is able to do this bc Route 53 has a relationship with all of the major domain registries: .com, .edu, .uk. .org, and so on.

Route 53 can also be used as Hosted Zones and also provides DNS zones and hosting for those zones. So route 53 is basically DNS as a service. Remember a Route 53 hosted zone is a DNS DB for a given section of the global DNS data for domains.

A hosted zone can also be private and linked to one or more VPCs and only accessible inside those VPCs.

Hosted Zones host our DNS records and record sets, and again that is A record, alias record, cname record, and so on.

Simple & Multi-Value routing policies
Let’s cover Route 53 routing policies. Routing policies are how route 53 responds to queries and which records get returned when users query domains. Route 53 offers simple routing, multi value, failover, weighted, latency and geolocation routing policies.

Simple routing policies work by configuring standard DNS records without special route 53 routing. So if we want to route traffic to www.amazon.com it is a single resource, so that query flows to the hosted zone database and that database has one record www. Which could have three values, and then all three of those are forwarded back to the client and one of the values one of those records is chosen at random and then the website is accessed.

But sometimes one of those records could be unhealthy so you user would receive an error instead of being directed through to the website.

And with simple routing policies, you cannot perform any granular health checking but you can with other routing policies and Multi value routing offers a solution to simple routing.

Multi value routine policies are similar to simple routing; however, simple routing has a key difference that you can have multiple records with the same name and each of these records can have a health check. So Route 53 will respond with all healthy record IP addresses so you get multi values but will remove any unhealthy records, so no unhealthy records make it through to your customer.

Multi value offers a solution to simple routing, but it is still a single record (set) that may have more than one value (record); by attaching health checks you can return only healthy values.

Failover routing Failover routing policies
Failover routing, you actually create two records with the same name and the same type and one is the primary and the other is the secondary

It is very similar to the simple routing policy that only has one record with one name. But with failover routing we have two records with the same name: so our primary record in this example could be a wordpress EC2 instance and your secondary record could be an EC2 instance or it could be the S3 endpoint URL from our S3 bucket hosting our static website. And we could use that S3 bucket for a static hosted error page; we would simply need to copy the S3 endpoint url.

So the point of failover routing is that if anything happens with our wordpress site that we created on our EC2 instance, then the route will failover to our secondary wordpress EC2 instance or even our S3 bucket hosting our ss static website.

And with failover routing we use health checks and each record has an associated healthcheck, so if the primary route is healthy then it is the one used. The secondary is only used when the primary record's health check fails.

Failover routing is used to implement active passive failover in DNS.

So with simple routing we cannot create multiple record sets with the same name but with failover we can And failover is great for HA.

Weighted routing policies
Weighted routing is a powerful routing policy and the way it works is you create multiple records with the same name within the hosted zone; however, each of those records you apply a weighted value, so maybe 50 50, or 75 25, or 90 10.  Weights can be assigned any number from 0 to 255. And the total percent weight is all the records added together and how often each record is returned on a DNS query is based on how heavily it is weighted.

And again you can use health checks so weighted routing policies are great for active/active failover, great for deployments; so you can add smaller percentage of request coming to the new application to see how it handles traffic and then eventually up that weight if it is working as needed and then remove the weight from the older application version.

And weighted routing is a really useful technique for all kinds of deployments. AWS give us multiple ways to do this: DNS is one of them, but we'll also see similar in EC2 load balancing.

And for simple traffic distribution, if you have services on a smaller EC2 instance, you can reduce the weight of traffic to that instance and have more weight going to a larger EC2 instance.

If you have migrations, it allows you to gradually move you load over.

Latency routing policies
Latency routing allows you to create multiple records with the same name and the same type.

For each record you specify a region for that record, and when a client request arrives, route 53 knows what region that request is coming from and also know the latency of that region and other regions as well and it will pick the healthy record with the lowest latency.

Latency Routing is a Public-Hosted Zone thing. It's possible to create within a private hosted zone, but doesn't really do anything. AWS has the ability to predict the likely latency for users based on their source IP address as long as it is a publically-routable address.

And I can add a like if you want to take a deeper dive.  More here: https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/resource-record-sets-values-latency.html

It is not based on geography, it is not a distant thing, it is based on latency.

Geolocation routing policies
Geolocation routing is focused on delivering queries to match the location of your customers, the physical geography. So you can create records with the same name and type in a hosted zone, but set a location field, so that location can be default, set to a country, or continent. So when a users queries for a record, Route 53 locates the location of that customer and then tries to match that location to a record in that county, if it cannot then it will try to achieve a continent match, and if cannot do either of those, then the default record if no other record applies is returned. If no record is located in that geolocation and no default record is listed then nothing is returned

If the records have a health check and the records are in an unhealthy state it will simply be passed over to the next record. Geolocation is designed to offer localized content to your customers by returning records in their geographic area, so those records can be in different languages to match those countries, etc. and priority also goes to the most specific record

A use-case of this is data protection/sovereignty issues for example Europe's general data protection regulation - and Geo-routing would be a great reason to use geo-location (as opposed to latency) to ensure the right EC2 instances, and databases, interact with European customers.

Types of DNS Records: CNAME vs Alias
A & AAAA
CNAME
TXT
MX
NS
In this lesson let's talk about the types of records that can be stored in DNS and Route 53. Without taking a deep dive it’s important to know that A and CNAME records are standard DNS records, whilst ALIAS records are custom DNS records.

A records

A records or AAAA records -  map host names to IP addresses,

A records map to IPv4 address and AAAA map to an IPV6 address

CNAME records, canonical name, for a given name the cname creates DNS short cuts, so host to host records. So if we have an A records pointed at our EC2 server for ss.com and maybe this server serves our website and performs multiple tasks, also receive emails from users, etc. so you can create three cname records to point to the one ec2 server A record, so all three CNAME resolve to the same IP address and CNAMEs can reduce your admin overhead. But CNAMEs cannot point directly to specific IP addresses only to other CNAMES or records.

Alias records

Amazon Route 53 alias records provide a Route 53–specific extension to DNS functionality. Alias records let you route traffic to selected AWS resources, such as CloudFront distributions and Amazon S3 buckets. They also let you route traffic from one record in a hosted zone to another record.

An alias record can only redirect queries to selected AWS resources, such as the following:

Amazon S3 buckets
CloudFront distributions
Another record in the same Route 53 hosted zone
For example, you can create an alias record named acme.example.com that redirects queries to an Amazon S3 bucket that is also named acme.example.com. You can also create an acme.example.com alias record that redirects queries to a record named zenith.example.com in the example.com hosted zone.

Understanding the differences

These are the main differences:

The A record maps a name to one or more IP addresses
The CNAME record maps a name to another name. It should only be used when there are no other records on that name. If the IP of the destination hostname changes, you won’t need to change your DNS records as the CNAME will have the same IP.
The ALIAS record maps a name to another name, but can coexist with other records on that name.

Important rules:

The A, CNAME, and ALIAS records cause a name to resolve to an IP. The A name must resolve to an IP. The CNAME and ALIAS records must point to a name.
MX Records are huge bc they help email on the internet work, so if you want to send an email, MX records are used as part of this process, so your email has to know what server to pass this email along to. MX records have a priority and a value, and the value can be a host or a fully qualified domain name, so it can point to a host in the same zone or to an outside zone, the priority value is used to choose which value to use

MX records use the SMTP protocol to deliver the mail

TXT records are also know as a text records and these allow you to add text to a domain, so the dns can provide additional functionality, and txt records can be added to our email to prove we own that domain

https://www.youtube.com/watch?v=HKh54BkaOK0&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=9

https://www.youtube.com/watch?v=6R44BADNJA8&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=8

Application Services
SQS
Let’s cover Amazon's Simple Queue Service, SQS and what you need to know about SQS for your exam. So what is SQS? Well, it is a queuing system that provides fully managed highly available message queues and SQS can be used for inter-process, servers, and services messaging.

So the way a que works, if you have a que, you add a message to the que, and then something else retrieves messages from that que, so it offers an asynchronous way to talk between two components of an application.

Exam tip: You may see a question in your exam regarding the sizes of SQS messages and each message can contain up to 256 KB of data.

And SQS has two types of polling, short and long polling.

Short polling is a single API call to check the que for any messages, and you will get the messages available in the que up to a max of 10 messages or you will get no messages. With short polling it responds immediately to any messages in the que, meaning you will need to constantly be sending API calls to check the queue for messages, and this consumes a lot of API calls.

But you can also use long polling, and this is the same process to check for messages in the que as short polling; however, you wait for a certain amount of time, and that time is known as the WaitTimeSeconds. So with long polling you can specify a time you are willing to wait until that que has messages, and then when messages arrive in your que, during the WaitTimeSeconds, those messages will be delivered to you immediately so you do not have to keep short polling that que for messages.

And long polling is more efficient because you have a lot less API calls to the queue but also a lot less empty API calls.

So when you have a message that is polled from the que, it is hidden in that que, they are not deleted, they are simply hidden for an amount of time, known as the VisibilityTimeOut, and when this time out periods expires: let’s say our visibility timeout period is 1 minute, then that hidden message will return to the que and then that message is visible to the que again after the time period.

So it is best practice to delete the message from the queue after that message has been polled and processed, and you may see a question regarding this in your exam.

SQS queues come in two different types: Standard and FIFO Queues

Standard was the AWS original and Fifo queues were added later but there are a few differences to know for your exam.

Standard queues are distributed and scalable to nearly an unlimited message volume, but the order of the message is not guaranteed, it is best-effort, and messages are guaranteed to be delivered at least once, but sometimes the messages are delivered more than once. You can have duplicate messages or out of order messages, but have great performance.

FIFO queues were introduced to solve this problem. FIFO stands for first in and first out and FIF ques guaranteed that messages are delivered in the order they were received, they are only ever  delivered once, so dupes do not occur.  BUT the throughput is limited to 300 messages without batching and 3000 messages per second with batching.

So let's talk about SQS' architecture, and SQS is used when you need to decouple two different parts of a system, and decouple is an exam keyword, so if you see decouple, asynchronous messaging, or the ability to have independent scaling of your application, on your exam, the correct answer will probably be SQS.

https://www.youtube.com/watch?v=8zysQqxgj0I&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=13

https://www.youtube.com/watch?v=o4clRJuH9xU&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=11

https://www.youtube.com/watch?v=EBSdyoO3goc&list=PLAJWTI4ZLaBVGQiPxLMpe6BAg5s5-SgbB&index=10

Logging and Security
Still to complete
