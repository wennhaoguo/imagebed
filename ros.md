# 

# ROS

## Basic concepts

1. Node : executable files, can be written by different languages

2. ROS master

   1. name and register nodes

   2. track and note topic, communication, find, connection

   3. save parameter, like a dictionary, the pic below, all yellow districts are nodes.![](/assets/images/image-20240110121145488-483x383.png)

3. Topic, tunnel of messages

   1. publisher

   2. subscriber

4. messages

   1. can be defined

5. Service![](/assets/images/image-20240110121829118-253x412.png)![](/assets/images/image-20240110121901990-857x447.png)

   1. use server and client

6. Parameter![](/assets/images/image-20240110122507737-737x347.png)

7. document system![](/assets/images/image-20240110122624192-621x370.png)

## ROS terminal commands

![](/assets/images/image-20240110122838710-1867x954.png)

1. roscore, start the ROS Master

2. rosrun package node

3. rqt_graph, show the compute graph

4. rosnode

   1. list

   2. info /node

5. rostopic

   1. list

   2. pub /topic_name tab show then modify

   3. pub -r, send with a certain frequency

6. reomsg show

7. rosservice

   1. líst

   2. call /service name tab

8. rosbag record -a -o cmd_record

   1. to record all the infos of current topic

   2. \-a all the infos

   3. \-o name it

9. rosbag play cmd_record.bag

   1. to show saved msgs

## start workspace and packages

![](/assets/images/image-20240110124437919-827x836.png)

![](/assets/images/image-20240110124246045-949x493.png)

1. set up workspace![](/assets/images/image-20240110124526789-1746x901.png)

2. set up packages![](/assets/images/image-20240110125859150-945x398.png)

3. check if the environment viarable

   1. echo $ROS_PACKAGE_PATH

## code of publisher

## Service and Topic,

1. client request, service response, then send messages through topic

2. server.cpp

   1. set up service name

   2. start server

   3. rosservice call the service name

   4. normally this service would be called in client

## Parameter and code

![](/assets/images/image-20240111111304601-688x418.png)

![](/assets/images/image-20240111111744437-642x92.png)

![](/assets/images/image-20240111111829086-688x380.png)

![](/assets/images/image-20240111112504814-946x803.png)

## TF

![](/assets/images/image-20240111132206117-1361x545.png)

`// 初始化ROS节点`

`ros::init(argc, argv, "mytfbroadcaster");`

in cpp files, the node was named as mytfbroadcaster, but the middle part of the above command, would rename the node.

/turtle1 is command parameter, to tell the cpp, that we want the node to subscribe which topic

![](/assets/images/image-20240111132517796-715x136.png)

# ros

Hello world!