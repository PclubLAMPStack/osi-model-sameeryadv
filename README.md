# OSI Model
OSI stands for Open Systems Interconnection. It describes 7 layers that computer system use to communicate over a network. **The modern Internet is not based on OSI model but on simpler TCP/IP model.**
## 7 Layers of OSI Model
We’ll describe OSI layers “top down” from the application layer that directly serves the end user, down to the physical layer.
![OSI Model 7 Layers](/img1.png)
### 7. Application Layer
This layer includes protocols like HTTP, POP, SMTP, DNS. This layer is used by end user application like browsers. It provide protocols that help application to send and receive data and present it in meaningful format.

### 6. Presentation Layer
This layer prepares data for application layer, it takes any data transmitted by application layer and prepares it for transmission over session layer. It defines how two devices encode, encrypt and compress data so that data can be received correctly at other end.

### 5. Session Layer
The session layer creates communication channels, called sessions, between devices. It is responsible for opening sessions, ensuring they remain open and functional while data is being transferred, and closing them when communication ends. The session layer can also set checkpoints during a data transfer—if the session is interrupted, devices can resume data transfer from the last checkpoint.

### 4. Transport Layer
The transport layer takes data transferred in the session layer and breaks it into “segments” on the transmitting end. It is responsible for reassembling the segments on the receiving end, turning it back into data that can be used by the session layer. The transport layer carries out flow control, sending data at a rate that matches the connection speed of the receiving device, and error control, checking if data was received incorrectly and if not, requesting it again.

### 3. Network Layer
The network layer has two main functions. One is breaking up segments into network packets, and reassembling the packets on the receiving end. The other is routing packets by discovering the best path across a physical network. The network layer uses network addresses (typically Internet Protocol addresses) to route packets to a destination node.

### 2. Data Link Layer
The data link layer establishes and terminates a connection between two physically-connected nodes on a network. It breaks up packets into frames and sends them from source to destination. This layer is composed of two parts—Logical Link Control (LLC), which identifies network protocols, performs error checking and synchronizes frames, and Media Access Control (MAC) which uses MAC addresses to connect devices and define permissions to transmit and receive data.

### 1. Physical Layer
The physical layer is responsible for the physical cable or wireless connection between network nodes. It defines the connector, the electrical cable or wireless technology connecting the devices, and is responsible for transmission of the raw data, which is simply a series of 0s and 1s, while taking care of bit rate control.