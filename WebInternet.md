

## **Unit 1 - Introduction to Web and Internet Technology**

### **Introduction**

Web and Internet technologies have revolutionized communication and business, creating a global network of interconnected systems. These technologies allow the sharing of information across multiple platforms, connecting users and services worldwide. The Internet itself is a network of networks that includes intranets, extranets, and the public Internet.

#### **Key Concepts:**

* **Network of Networks**: The Internet connects millions of networks across the globe.
* **Intranet**: A private network used within an organization, utilizing Internet protocols for internal communications.
* **Extranet**: A private network that allows controlled access to outsiders, such as partners or vendors.
* **Internet**: A public global network that facilitates worldwide information sharing and communication.

---

### **World Wide Web (WWW)**

The World Wide Web (WWW) is a system of interlinked hypertext documents accessed via the Internet. It allows users to navigate between documents by following hyperlinks, enabling access to web pages, multimedia, and interactive content.

#### **Key Concepts:**

* **Domain and Subdomain**: Domains (like example.com) represent addresses for websites, while subdomains (e.g., blog.example.com) are divisions within the domain.
* **Address Resolution**: The process of converting human-readable domain names into machine-readable IP addresses using DNS (Domain Name System).
* **DNS (Domain Name System)**: A hierarchical system that maps domain names to IP addresses, ensuring users can access websites using easily recognizable names.
* **Telnet**: A protocol that allows users to log into remote computers over the network using a command-line interface.
* **FTP (File Transfer Protocol)**: A protocol used to transfer files between a client and a server on the Internet.
* **HTTP (Hypertext Transfer Protocol)**: A protocol used for transferring web pages from a server to a browser. It is stateless, meaning each request is independent and does not rely on previous interactions.

---

### **Review of TCP/IP**

TCP/IP is the fundamental suite of protocols that supports Internet communications. It enables data exchange between computers on a network by breaking data into smaller packets, transmitting them, and reassembling them at the destination.

#### **Key Concepts:**

* **Features of TCP/IP**:

  * **Segment**: A unit of data at the transport layer of TCP/IP.
  * **Three-Way Handshaking**: A process for establishing a TCP connection, which involves sending and acknowledging SYN and ACK packets.
  * **Flow Control**: Ensures that data is transferred at an optimal rate to prevent network congestion.
  * **Error Control**: Ensures data integrity by detecting and correcting transmission errors.
  * **Congestion Control**: Avoids network congestion by adjusting the rate of data transmission.
  * **IP Datagram**: A packet structure used for routing data across the Internet.
  * **IPv4 and IPv6**: IPv4 uses a 32-bit address, while IPv6 uses a 128-bit address, offering a vastly larger address space.

---

### **IP Subnetting and Addressing**

IP addressing is crucial for network identification, and subnetting divides networks into smaller, more manageable segments, improving routing efficiency and security.

#### **Key Concepts:**

* **Classful and Classless Addressing**: Classful addressing (A, B, C) is based on predefined classes, while classless addressing (CIDR) allows for more flexible subnetting.
* **Subnetting**: The process of dividing a network into smaller sub-networks (subnets), optimizing network performance and security.
* **NAT (Network Address Translation)**: A method of modifying the IP address information in packet headers as they pass through a router or firewall, allowing multiple devices within a private network to share a single public IP address.
* **IP Masquerading**: A form of NAT where the source IP address of outgoing packets is replaced by the public IP address of the router.
* **IP Tables**: A firewall feature in Linux that allows for packet filtering, network address translation (NAT), and other network management tasks.

---

### **Internet Routing Protocol**

Routing protocols are responsible for determining the best paths for data to travel through networks.

#### **Key Concepts:**

* **Intra and Inter Domain Routing**: Intra-domain routing (e.g., RIP, OSPF) operates within a single network domain, while inter-domain routing (e.g., BGP) manages routing between different domains.
* **Unicast, Multicast, and Broadcast Routing**:

  * **Unicast**: One-to-one communication between a sender and a receiver.
  * **Multicast**: One-to-many communication, where data is sent to multiple recipients who are part of a group.
  * **Broadcast**: One-to-all communication, where data is sent to all devices within a network.

---

### **Electronic Mail**

Email protocols enable the sending, receiving, and storage of electronic messages.

#### **Key Concepts:**

* **POP3 (Post Office Protocol version 3)**: A protocol for retrieving emails from a server. It downloads emails to the client device and removes them from the server.
* **SMTP (Simple Mail Transfer Protocol)**: A protocol for sending email messages from the client to the server, and between email servers.

---

## **Unit 2 - HTML, XML, and CGI Scripts**

### **HTML (3L)**

#### **Introduction to HTML**

HTML (HyperText Markup Language) is the standard language used for creating and structuring web pages. It defines the structure and layout of a web document by using various tags and attributes.

#### **Editors**

HTML can be written using any text editor (like Notepad, Sublime Text, Visual Studio Code) or specialized HTML editors (like Dreamweaver).

#### **Elements and Attributes**

* **Elements**: HTML elements consist of tags that define content. Each element has an opening tag (e.g., `<h1>`) and a closing tag (e.g., `</h1>`), with content in between.
* **Attributes**: Provide additional information about elements. For example, in `<img src="image.jpg" alt="Description">`, `src` and `alt` are attributes.

#### **Common HTML Elements**:

* **Heading**: `<h1>`, `<h2>`, ... `<h6>` elements are used to define headings of different sizes.
* **Paragraph**: `<p>` tag defines a block of text as a paragraph.
* **Formatting**: Text formatting tags like `<b>` for bold, `<i>` for italic, and `<u>` for underline.
* **Link**: The `<a>` tag is used to create hyperlinks. Example: `<a href="https://www.example.com">Click Here</a>`.
* **Head**: The `<head>` section contains meta-information about the document like the title, character encoding, and linked CSS files. Example: `<head><title>Page Title</title></head>`.
* **Table**: The `<table>` tag is used to create tables, with `<tr>` for rows, `<th>` for table headers, and `<td>` for table data cells.
* **List**: HTML provides two types of lists:

  * **Ordered List**: `<ol>` creates a numbered list, and `<li>` is used for list items.
  * **Unordered List**: `<ul>` creates a bulleted list, and `<li>` defines list items.
* **Block Layout**: Elements like `<div>` are block-level elements that typically take up the full width of their container.
* **CSS**: CSS (Cascading Style Sheets) is used to style HTML elements (colors, fonts, layout). External stylesheets are linked using `<link>` in the `<head>` section.
* **Form**: The `<form>` tag is used for creating interactive forms to collect user input. Form elements include `<input>`, `<textarea>`, `<select>`, and `<button>`.
* **Iframe**: The `<iframe>` tag allows embedding another HTML document within the current document, often used for embedding external content like videos.
* **Colors**: HTML supports color specification in various formats like:

  * **Colorname**: Common color names (e.g., `red`, `blue`, `green`).
  * **Colorvalue**: RGB values (e.g., `rgb(255,0,0)` for red) and Hexadecimal values (e.g., `#ff0000` for red).

---

### **Image Maps (1L)**

#### **Introduction to Image Maps**

An image map allows specific areas of an image to act as hyperlinks. Instead of making the whole image clickable, image maps let you define clickable regions, often used for navigation menus, image galleries, and diagrams.

#### **Map and Area**

* **`<map>`**: The `<map>` tag defines the image map. It contains one or more `<area>` tags that specify the clickable areas.
* **`<area>`**: Defines a specific area within the image map. Attributes of `<area>` include:

  * **shape**: Defines the shape of the area (`rect`, `circle`, `poly`).
  * **coords**: Specifies the coordinates for the clickable area.
  * **href**: The URL that the area links to.
  * **alt**: Alternative text for the area.

Example of an image map:

```html
<map name="image-map">
  <area shape="rect" coords="34,44,270,350" href="https://www.example.com" alt="Link 1">
  <area shape="circle" coords="150,150,50" href="https://www.example2.com" alt="Link 2">
</map>
<img src="image.jpg" usemap="#image-map" alt="Image Map">
```

---

### **Extensible Markup Language (XML) (4L)**

#### **Introduction to XML**

XML (Extensible Markup Language) is a flexible text format used to store and transport data. Unlike HTML, XML does not define how the data is displayed but focuses on the structure and meaning of the data.

#### **XML Tree Structure**

* **Root Element**: The top-level element that contains all other elements in the XML document.
* **Child Elements**: Elements nested within the root or other elements, forming a tree-like structure.

#### **Syntax**

* XML documents are case-sensitive.
* Tags must be properly nested and closed.
* The document must have one root element.
* Data is stored between opening and closing tags.

#### **Elements and Attributes**

* **Elements**: Represent data in the XML structure.
* **Attributes**: Provide additional information about an element.

#### **Validation**

* XML documents can be validated against a **DTD (Document Type Definition)** or **XSD (XML Schema Definition)** to ensure they adhere to a specific structure and data types.

#### **Viewing XML**

* XML documents can be viewed in browsers or text editors, but browsers do not display them with a layout. They only display the raw data.

#### **XHTML in Brief**

* XHTML (Extensible HTML) is a stricter version of HTML based on XML. It requires properly closed tags and the use of lowercase elements, making it more structured and less forgiving than HTML.

---

### **CGI Scripts (1L)**

#### **Introduction to CGI**

CGI (Common Gateway Interface) is a standard for running external programs on a web server to generate dynamic content. CGI scripts process user input and interact with databases or other back-end systems to create dynamic responses.

#### **Environment Variables**

* CGI scripts can access environment variables provided by the web server, such as `REQUEST_METHOD`, `QUERY_STRING`, and `REMOTE_ADDR`, to obtain information about the request and client.

#### **GET and POST Methods**

* **GET**: Sends data in the URL, typically used for retrieving data or non-sensitive requests.
* **POST**: Sends data in the HTTP body, often used for submitting form data, as it is more secure for large or sensitive data.

Example of a simple CGI script in Python:

```python
#!/usr/bin/env python
import cgi
print("Content-type: text/html\n")
form = cgi.FieldStorage()
name = form.getvalue("name")
print(f"<h1>Hello, {name}!</h1>")
```

---

## **Unit 3 - PERL, JavaScript, Cookies, Java Applets, and Client-Server Programming in Java**

### **PERL (3L)**

#### **Introduction to PERL**

PERL (Practical Extraction and Report Language) is a high-level, general-purpose programming language designed for text processing, report generation, and quick scripting. It's widely used in web development, system administration, and data manipulation.

#### **Variables**

* **Scalar Variables**: Used to store single values (strings, integers, or floating-point numbers), prefixed with `$` (e.g., `$variable`).
* **Array Variables**: Used to store ordered lists, prefixed with `@` (e.g., `@array`).
* **Hash Variables**: Used to store key-value pairs, prefixed with `%` (e.g., `%hash`).

#### **Conditionals**

* **If-else**: Used for conditional execution of code.

  ```perl
  if ($x > 10) {
      print "x is greater than 10";
  } else {
      print "x is less than or equal to 10";
  }
  ```

#### **Loops**

* **For loop**: Iterates over a range of values or an array.

  ```perl
  for (my $i = 0; $i < 10; $i++) {
      print "$i\n";
  }
  ```
* **While loop**: Repeats as long as the condition is true.

  ```perl
  while ($x < 10) {
      $x++;
  }
  ```

#### **Arrays**

Arrays store lists of data, and elements are accessed using indices (e.g., `$array[0]`).

* **Array Operations**: `push`, `pop`, `shift`, `unshift`, `splice`.

#### **Implementing Data Structures**

* **Hash (Associative Array)**: Useful for storing key-value pairs, accessed with keys (e.g., `$hash{"key"}`).
* **String Operations**: PERL provides various string manipulation functions like `substr`, `index`, `split`, and `join`.

#### **Regular Expressions**

Regular expressions are powerful tools for pattern matching and text processing in PERL.

* Example:

  ```perl
  if ($string =~ /pattern/) {
      print "Pattern found!";
  }
  ```

#### **File Handling and I/O**

PERL provides functions for reading, writing, and manipulating files:

* **open**: Opens a file for reading or writing.
* **read** and **write**: Handle data read and write operations.
* **close**: Closes a file handle.

---

### **JavaScript (4L)**

#### **Basics of JavaScript**

JavaScript is a client-side scripting language used for adding interactivity and dynamic behavior to web pages.

#### **Statements**

JavaScript statements are the instructions that perform actions, such as defining variables, performing calculations, or manipulating the DOM.

#### **Comments**

* **Single-line comment**: `// This is a comment`
* **Multi-line comment**: `/* This is a comment */`

#### **Variables**

Variables are defined using `var`, `let`, or `const`, depending on the scope and mutability:

* `var` is function-scoped (legacy).
* `let` and `const` are block-scoped.

#### **Comparison Operators**

* **Equality**: `==` (checks value), `===` (checks value and type).
* **Inequality**: `!=`, `!==`.
* **Greater than/less than**: `>`, `<`, `>=`, `<=`.

#### **Conditional Statements**

* **If-else**: Executes code based on conditions.

  ```javascript
  if (x > 10) {
      console.log("x is greater than 10");
  } else {
      console.log("x is less than or equal to 10");
  }
  ```

#### **Switch Statement**

A cleaner alternative to multiple `if-else` statements for checking multiple conditions.

```javascript
switch (day) {
    case 1:
        console.log("Monday");
        break;
    case 2:
        console.log("Tuesday");
        break;
    default:
        console.log("Invalid day");
}
```

#### **Loops**

* **For loop**: Iterates over a set range or collection.
* **While loop**: Repeats as long as the condition is true.
* **For...in loop**: Loops over object properties.
* **For...of loop**: Loops over iterable objects like arrays.

#### **Objects**

* **String**: An object representing a sequence of characters, with methods like `length`, `toUpperCase()`, and `slice()`.
* **Array**: An ordered collection of items, with methods like `push()`, `pop()`, `shift()`, and `map()`.
* **Boolean**: Represents `true` or `false` values.
* **RegEx (Regular Expression)**: A powerful tool for matching patterns within strings.

#### **Functions**

Functions in JavaScript can be defined using `function` keyword or as arrow functions (`() => {}`).

```javascript
function greet(name) {
    console.log("Hello, " + name);
}
```

#### **Errors and Validation**

* JavaScript includes error handling using `try`, `catch`, and `finally`.
* Validates form data (like ensuring that input fields are not empty) before submitting using `onsubmit`.

---

### **Cookies (1L)**

#### **Definition of Cookies**

Cookies are small pieces of data stored by a browser that can hold user-specific information like preferences, authentication details, or tracking information.

#### **Creating and Storing a Cookie**

Cookies are created using `document.cookie` and can be stored with attributes like expiration date, domain, and path.

```javascript
document.cookie = "username=JohnDoe; expires=Thu, 18 Dec 2025 12:00:00 UTC; path=/";
```

---

### **Java Applets (2L)**

#### **Container Class**

In Java, an Applet runs inside a container (like a browser or an applet viewer) that manages its lifecycle and communicates with the Java runtime environment.

#### **Components of an Applet**

An applet consists of methods for initialization (`init()`), starting (`start()`), stopping (`stop()`), and cleaning up (`destroy()`).

#### **Applet Life Cycle**

1. **Initialization (`init()`)**: Initializes the applet; called once when the applet is loaded.
2. **Start (`start()`)**: Called after `init()` and whenever the applet is brought to the foreground.
3. **Stop (`stop()`)**: Called when the applet is no longer visible.
4. **Destroy (`destroy()`)**: Called before the applet is unloaded.

#### **Update Method**

The `update()` method is used for efficient redrawing of the applet when it changes its display.

#### **Parameter Passing in Applets**

Parameters can be passed to applets using the `<param>` tag within the `<applet>` tag. These parameters can be accessed inside the applet using the `getParameter()` method.

#### **Applications of Applets**

Applets were traditionally used for tasks such as displaying graphics, creating interactive elements, and performing calculations on the client side. However, their use has declined with the rise of JavaScript and other web technologies.

---

### **Client-Server Programming in Java (2L)**

#### **Client-Server Architecture**

Java-based client-server programming allows communication between a client (usually a web browser) and a server (Java application).

#### **Sockets in Java**

Java provides the `java.net` package to handle client-server communication using sockets.

* **Client**: The client connects to the server using `Socket` class.
* **Server**: The server listens for incoming requests using `ServerSocket` class.

Example of a simple Java server-client model:

* **Server**:

  ```java
  ServerSocket server = new ServerSocket(1234);
  Socket clientSocket = server.accept();
  BufferedReader input = new BufferedReader(new InputStreamReader(clientSocket.getInputStream()));
  ```

* **Client**:

  ```java
  Socket socket = new Socket("localhost", 1234);
  PrintWriter out = new PrintWriter(socket.getOutputStream(), true);
  out.println("Hello Server!");
  ```

---



## **Unit 4 - Java Socket, Java RMI, Network Security, Firewall, Internet Telephony, Multimedia Applications, and Search Engine**

### **Java Socket and Java RMI**

#### **Java Socket**

Java Sockets provide the foundation for communication between applications over a network. It allows communication between two devices or applications, enabling data transmission between them using TCP/IP or UDP protocols.

* **Client-Side Socket**: The client creates a socket to communicate with the server.

  ```java
  Socket socket = new Socket("localhost", 1234);
  ```
* **Server-Side Socket**: The server listens for incoming requests using `ServerSocket` and establishes a communication link with the client.

  ```java
  ServerSocket serverSocket = new ServerSocket(1234);
  Socket clientSocket = serverSocket.accept();
  ```

#### **Java RMI (Remote Method Invocation)**

Java RMI allows invoking methods of an object that resides in a different JVM, providing the foundation for distributed applications.

* **RMI Components**:

  * **Stub**: A proxy object that represents the remote object on the client side.
  * **Skeleton**: The server-side object that receives requests from the client and dispatches them to the actual object.
  * **Registry**: Used to look up remote objects.

* **RMI Example**: The client makes a request to invoke a method on a remote object via the RMI registry.

  ```java
  MyRemoteObject obj = (MyRemoteObject) Naming.lookup("rmi://localhost/MyRemoteObject");
  obj.remoteMethod();
  ```

---

### **Threats (1L)**

#### **Malicious Code**

* **Viruses**: Self-replicating programs that attach themselves to legitimate programs and spread when those programs are executed.
* **Trojan Horses**: Malicious programs disguised as legitimate software, typically used for unauthorized access to systems.
* **Worms**: Self-replicating programs that spread across networks without the need to attach to other programs, consuming resources and bandwidth.

#### **Eavesdropping**: Unauthorized interception of network traffic to obtain sensitive information, such as passwords or private communications.

#### **Spoofing**: An attacker impersonates another user or device to gain unauthorized access or perform malicious activities.

#### **Modification**: Attackers alter the contents of communications or data packets in transit, potentially changing their meaning or redirecting information.

#### **Denial of Service (DoS)**: An attack that disrupts the availability of a network service by overwhelming it with excessive traffic or by exploiting system vulnerabilities to crash or hang the service.

---

### **Network Security Techniques (2L)**

#### **Password and Authentication**

* **Password Protection**: Secures user access by requiring authentication with a password.
* **Authentication Methods**: Includes techniques such as biometrics, smart cards, and two-factor authentication for verifying identity.

#### **VPN (Virtual Private Network)**

A VPN creates a secure, encrypted tunnel over the Internet, allowing users to send and receive data as though they were directly connected to a private network.

* **Types of VPN**:

  * **Remote Access VPN**: Provides secure access for remote users to a corporate network.
  * **Site-to-Site VPN**: Connects entire networks over the Internet securely.

#### **IP Security (IPsec)**

IPsec is a suite of protocols designed to secure Internet Protocol (IP) communications by authenticating and encrypting each IP packet in a communication session.

#### **Security in Electronic Transactions**

Ensures secure online transactions through encryption, authentication, and integrity checks to protect financial and personal data.

#### **SSL (Secure Socket Layer)**

SSL is a protocol that ensures secure data transmission between a web server and a client by encrypting communication.

* **SSL/TLS**: The successor of SSL, providing more robust encryption for secure communications.

#### **SSH (Secure Shell)**

SSH is a cryptographic network protocol for securing communication between two networked computers, primarily used for secure remote login and data transfer.

---

### **Firewall (1L)**

#### **Introduction to Firewalls**

A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predetermined security rules. It can be hardware, software, or a combination of both.

#### **Types of Firewalls:**

* **Packet Filtering**: Inspects packets at the network layer. It filters traffic based on IP addresses, ports, and protocols.
* **Stateful Inspection**: Monitors the state of active connections and makes decisions based on the state of the connection.
* **Application Layer**: Operates at the application layer to inspect and filter specific applications or services (e.g., HTTP, FTP).
* **Proxy Firewall**: Acts as an intermediary between users and the services they access, forwarding requests on behalf of users while filtering and controlling access.

---

### **Internet Telephony (1L)**

#### **Introduction to VoIP (Voice over Internet Protocol)**

VoIP is a technology that allows voice communication and multimedia sessions over the Internet, bypassing traditional telephone networks.

* **VoIP Protocols**: Includes protocols such as SIP (Session Initiation Protocol) and RTP (Real-Time Transport Protocol) for transmitting audio and video.

---

### **Multimedia Applications (2L)**

#### **Multimedia over IP**

Multimedia applications involve the transmission of audio, video, and other multimedia content over IP-based networks.

* **RSVP (Resource Reservation Protocol)**: A protocol for reserving resources across a network to ensure QoS (Quality of Service) for multimedia applications.
* **RTP (Real-Time Transport Protocol)**: A protocol used for delivering multimedia over IP networks, providing timing and sequencing.
* **RTCP (RTP Control Protocol)**: Works alongside RTP to monitor transmission statistics and provide feedback on quality.
* **RTSP (Real-Time Streaming Protocol)**: Used for streaming audio and video over the Internet, providing controls like pause, play, and seek.

#### **Streaming Media**

* Streaming refers to the continuous delivery of multimedia content over a network, typically through services like YouTube, Netflix, etc.
* **Codecs**: Compression-decompression algorithms used for encoding and decoding audio and video files (e.g., H.264 for video, MP3 for audio).
* **Plugins**: Small software components that add functionality to a web browser, such as Flash or Silverlight, enabling multimedia content playback.
* **IPTV (Internet Protocol Television)**: A system for delivering television content over Internet Protocol (IP), rather than traditional satellite or cable systems.

---

### **Search Engine and Web Crawler (2L)**

#### **Search Engine**

A search engine is a tool that helps users find information on the Internet by indexing web pages and providing search results based on keywords and algorithms.

#### **Web Crawlers**

* **Web Crawler**: An automated program (or bot) that browses the web and indexes content for search engines. It follows links from page to page, gathering data along the way.

#### **Meta Data**

Metadata is data that provides information about other data. In the context of web pages, it can include descriptions, keywords, and author information, which help search engines index pages more effectively.

#### **Indexing**

Indexing is the process of organizing data so that it can be quickly retrieved by search engines. Crawlers use indexing to understand the content of web pages and display relevant results.

#### **Page Rank**

PageRank is an algorithm used by Google to rank web pages based on their link structure. Pages with more inbound links from trusted sources tend to rank higher in search results.

#### **Overview of SEO (Search Engine Optimization)**

SEO is the practice of optimizing web pages to improve their visibility in search engine results. It involves strategies like keyword optimization, backlinking, and content quality enhancement to improve search rankings.

---
