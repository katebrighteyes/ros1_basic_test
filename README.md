# ros1_basic_test

## .bashrc 확인

gedit .bashrc

## Topic Test

<새터미널> 

roscore

<새터미널> 

rosrun ros_basic_test rostopic_pub.py

<새터미널> 

rosrun ros_basic_test rostopic_sub.py

<새터미널> 

rosnode list

rostopic list

rostopic echo /counter

* 모든 창을 닫아주세요

## Customed Message Topic Test

<새터미널>

roscore

<새터미널>

rosrun ros_basic_topicmsg info_publisher.py

<새터미널>

rosrun ros_basic_topicmsg info_subscriber.py

<새터미널>

rosnode list

rostopic list

rostopic echo /counter

rqt_graph

## launch

roslaunch ros_basic_topicmsg launch_test.launch

* 모든 창을 닫아주세요

## Service Test

<새터미널> 

roscore

<새터미널> 

rosrun ros_basic_service srv_server.py

<새터미널> 

rosrun ros_basic_service srv_client.py Hello my friend

<새터미널> 

rosservice list

rosservice info /word_counter

rosservice call /word_counter "Hello my friend?"

* 모든 창을 닫아주세요

## Action Service Test (기본)

<새터미널> 

roscore

<새터미널> 

rosrun ros_basic_action simple_action_server.py

<새터미널> 

rosrun ros_basic_action simple_action_client.py

<새터미널> 

rostopic list

* 모든 창을 닫아주세요

## Action Service Test (full)

<새터미널> 

roscore

<새터미널> 

rosrun ros_basic_asynctest async_action_server.py

<새터미널> 

rosrun ros_basic_asynctest async_action_client.py

<새터미널> 

rostopic list

* 모든 창을 닫아주세요
