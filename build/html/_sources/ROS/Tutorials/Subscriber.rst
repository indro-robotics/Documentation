.. toctree::
   :hidden:


Subscriber
================


**WHAT IS A ROS SUBSCRIBER**

A subscriber is the other end of a publisher node. While a publisher releases data on a topic, if a subscriber is listening to that topic, it can receive all the data the publisher is releasing. To


**CREATE A SUBSCRIBER**

Subscriber code is very similar to publisher code. The subscriber is going to be a python file created in the scripts folder of your chosen ROS package. The following picture is a template of what a subscriber could look like. 

.. code-block::
	
	#/usr/bin/env python
	import rospy
	from std_msgs.msg import String
	
	def callback_receive_data(msg):
		rospy.loginfo("Message received: ")
		rospy.loginfo(msg)
	
	if __name__ == '__main__':
		rospy.init_node('subscriber_name')
		sub = rospy.Subscriber("name_of_Topic", String, callback_receive_data)
		
		rospy.spin() #keep the script waiting for the callback


we have created a subscriber out of the subscriber class, with a topic name (should match publisher topic name if you want them to comunicate), the data type (string) and a function call that handles the data transmission.

The rospy.spin() function is also an important step in the code. It allows the code to stop and wait on that spot. Otherwise, the script would end, and the node might shut down before even receiving anything from the publisher.

Running the code with a publisher of the same topic, the output should look like the following.

.. image:: subscriber.gif
	:width: 700
	:alt: Directory Layout


