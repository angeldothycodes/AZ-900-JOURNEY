

Small exercise: let's imagine we are a startup company and we want to host our own application and build entire infrastructure for that reason. First thing we will need to do that is to purchase some servers. All the hardware that will actually run the applications themselves. Obviously, our servers needs to be able to connect to the Internet, therefore, we will need to provide all the networking infrastructure including the Internet connectivity itself. Because every server needs a storage, you will need to additionally provide a storage infrastructure. And those are hard drives or SSD, some RAID arrays, etc.

![Uploading Screenshot 2025-06-05 210447.png…]()


Once this is in place, you have all the hardware needed in order to run the server. In order to ensure the best utilization of the hardware that you have, you will want to run some virtualization to run mutiple virtual machine on a single hardware piece to host multiple applications but still maintaining the separations of the environemnts. All those virtual machines will needs an operating systems (Windows, Linux, or any other OS on the market), a middleware which typically means all the software additions that you need in order to run the system and the application itself. A typical application will additionally need a runtime- if this is a web application this could be IES web container, if it's a container application then maybe Docker. But runtime is additional layer that you will need to maintain yourself. Once those layers are in place, we are now finally ready to host our application and application data on that system. 


