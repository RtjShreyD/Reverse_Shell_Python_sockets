#### Reverse Shell

##### The project here demonstrates the operation of a Revershe shell in networking. It is basically a reverse connection between a client's system to the server which is being managed by the server, eg a Hacker uses reverse shell to break into victim's computer and do anything via the command line, which is demonstrated here. A Reverse shell works on Sockets and this is a very basic implementation of Reverse shell client-server system using Socket programming in Python3.

__Testing on localhost__

In the `client.py` file in the host variable put the IP address of the host, here `127.0.0.1`, then
run, `python3 server.py` in one terminal and `python3 client.py` in another terminal.
After connection established, terminal commands can be sent from server to the client which will work as desired on the client's system.


__Testing in a global network__

Start a cloud server instance preferrably a Linux instance, AWS EC2 recommended, you can follow AWS docs, https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html .

Once an Ubuntu Linux Instance is running and you are connected to it via ssh, use `nano server.py` to create a new file named server.py and copy the contents of server.py into it and save it.
Finally run, `python3 server.py` on the EC2 instance. A socket server gets started and is ready to accept connections.

In the `client.py` file in the host variable put the IP address of the host is `<public IP of the cloud instance>`
run, `python3 client.py` on a client's terminal which could be victim's system or any.
After connection established, terminal commands can be sent from server to the client which will work as desired on the client's system.

###### For reference,
https://www.youtube.com/playlist?list=PLhTjy8cBISErYuLZUvVOYsR1giva2payF
