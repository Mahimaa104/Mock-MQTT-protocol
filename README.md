# Mock-MQTT-protocol
Publisher-Subscriber Model Simulation

**MQTT**, which stands for *Message Queuing Telemetry Transport*, is a lightweight and open-source messaging protocol designed for efficient communication between devices in scenarios with limited bandwidth, high latency, or unreliable networks. 
MQTT follows a publish-subscribe architecture. Devices can act as publishers that send messages, and others can subscribe to receive specific types of messages. It supports asynchronous communication, allowing devices to send and receive messages independently of each other.

This code implements a simple simulation of an MQTT broker and clients in **Python**. 
The broker (broker.py) is responsible for handling communication between publishers and subscribers. It uses UDP sockets and multithreading for concurrent handling of messages. Publishers (publisher.py) and subscribers (subscriber.py) are client implementations interacting with the broker to publish and subscribe to topics, respectively.
The template.py provides a base class for common functionalities, and the client.py class defines a basic client structure. The simulation allows publishers to send data to specified topics, subscribers to receive data from subscribed topics, and the broker to manage these communications.

**HOW TO RUN**
**Broker:**
Open a terminal and navigate to the directory containing broker.py.
Run the broker script using the following command:

*python broker.py*

The broker will start listening for incoming messages on the specified IP address and port.

**Publisher:**
Open a new terminal and navigate to the directory containing publisher.py.
Run the publisher script using the following command:

*python publisher.py*

Enter a topic and data when prompted to publish a message.

**Subscriber:**
Open another terminal and navigate to the directory containing subscriber.py.
Run the subscriber script using the following command:

*python subscriber.py*

Enter a topic when prompted to subscribe to messages.
