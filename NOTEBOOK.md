# Progress Notes for I523-E534 : Big Data Applications and Big Data Applications Analytics
# Week 08/20/18 - 08/31/18
* requested access to canvas 
* reviewed course material and the reading for the first week
* researched IEEE Bio 
* wrote a Bio for  and posted it to Piazza
* setup GIThub account and wrote up notes of class progress

# Week Fri 08/31/18 - 09/06/18

* Read through EPUB text book up to section 4.4 and watched many of the videos
* joined cloudmesh-community from email invite
* worked to gain familiarity with github

*TODO 
Take Plagarism Certification Test, Setup VM - Linux


compare to other GUI streamers 

NIFI


## Google Kubernetes :smiley: fa18-523-56

|          |                       |
| -------- | --------------------- |
| title    | Google Kubernetes     | 
| status   | 90                    |
| section  | DevOps                |
| keywords | DevOps                |



### Kubernetes

Google Kubernetes is a cluster management platform developed by Google. Since 2014 Kubernetes has been open source and managed by The Cloud Native Computing Foundation[@fa18-523-56-www-kubernetes.io]. Kubernetes is popular because of its flexibility and powerful capabilities to meet the demands of modern cloud-based architecture. Kubernetes is the result of efforts at Google to manage containers with hallmarks of both Infrastructure as a Service and Platform as Service.  Building Kubernetes, google engineers had some specific goals; 

> "...make it easy to deploy and manage complex distributed systems, while still benefiting from the improved utilization that containers enable." [@fa18-523-56-www-3google-containers-mgmt-sys]

### What is Kubernetes

So what is Kubernetes? In simple terms Kubernetes intended be the central platform and managing entity for applications, tools and workloads in any environment. Kubernetes is geared towards container  environments where workloads go up and down. Kubernetes can organize and balance the connectivity, disk space and distributed computing in a containerized infrastructure.  [@fa18-523-56-www-kubernetes.io]

### Flexibility and Extensibility

Kubernetes is not limited to the cloud, but it seeks to be at the forefront of cloud architecture. Flexibility and extensibility are key Kubernetes hallmarks. The goal with Kubernetes is to allow as many other solutions to be used in the infrastructure as possible.  Kubernetes is intended to be extremely flexible. With this goal it doesn't dictate a CI or automation policy. It allows the user to build a container in a way that best serves the organizations needs then provides the management tools to scale, manage, and maintain that complex cloud based applications or infrastructure.  

### Kubernetes Key Components 

Kubernetes can be broken into two architectural buckets; the master node and workers notes. Within the master node as you might expect one of the key components is the API server. The API server controls the cluster and executes REST commands. Scheduled jobs and activities are initiated from the API server via the scheduler. 

Outside of the master node are the worker nodes. Pods are run in the worker nodes. Pods are run on the same host and can contain a group of containers that work together. Pods share volumes and network connectivity and other resources.  Kubelets receive from the API server configuration info for the pod.


## Protobuf :smiley: fa18-523-56


|          |                            |
| -------- | -------------------------- |
| title    | Protobuf                   | 
| status   | 90                         |
| section  | Message and Data Protocols |
| keywords | Message and Data Protocols, RPC, xml  |



### Protocol Buffer 

Protocol Buffer is a way to serialize structured data into binary form in order to transfer it over wires or for storage. [@www-protobuf] It is used for inter application communication or for remote procedure call (RPC). It involves an interface description that describes the structure of some data and a program that can generate source code or parse it back to the binary form. It emphasizes simplicity and performance. Protocol Buffer allows user to define the schema for their data and put messages within the schema. [@fa18-523-56-www-protobuf-codeclimate-chooseprobuf]

### Protocol Buffer Languages

Protocol Buffers has APIs for Python, Java, and C++ and other projects are in the works to implement other languages as well. [@fa18-523-56-www-protobuf-googleother] Protocol Buffer defines it’s schema definition in the .proto and is built with key/value pairs. 

### Protocol Buffer and xml

Protocol Buffers is compared frequently to xml. The tradeoff between xml and protocol buffers is read ability and speed/size. Protocal buffers are typically smaller, faster but require the consumer to have the protocol file to de-serialize the data. [@fa18-523-56-www-protobuf-googledevoverview] xml provides the information needed to parse but is typically slower to parse and transmit because of its size difference to Protocol Buffers. [@fa18-523-56-www-protobuf-performancecompare]

### Protocol Buffer History 

Protocol Buffers was developed by Google and by 2008 was primary in much of Google’s infrastructure. In 2008 Google made Protocol Buffers available open source. The project is available at https://github.com/protocolbuffers/protobuf

### Protocol Buffers and Large Files

Protocol Buffers wasn’t intended to deal with larger files. [@fa18-523-56-www-protobuf-googletechniques] Big data challenges frequently include larger files. However, Protocol Buffers is ideal for smaller structured pieces of a larger message. For example Google Maps files includes large amounts of data, but Protocol Buffers is the ideal solution because loading a large amount of data in small pieces is what where Protocol Buffers can excel.
