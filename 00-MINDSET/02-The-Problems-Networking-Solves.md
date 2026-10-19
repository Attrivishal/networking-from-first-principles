## 1. Objective 
  
  The objective of this document is to understand the fundamental engineering problems that arise when independent computing systems communicate. 

  Before learning individual networking technologies, we must understand the requirements that those technologies were designed to satisy. 

  A network is not simply a collection of connected computers. It is a communication system that must solve several interdependent problems involving transmission, identification, delivery, addressing, routing, application communication, reliability, security, and observability.

  By the end of this document, you should be able to explain:

     
        - Why communication requires a transmission medium.

        - Why transmitted information needs a defined representation.

        - Why a destination must be identified.

        - Why identifying a machine is different from identifying an application.

        - Why local delivery and remote delivery are different problems.

        - Why large networks need forwarding and routing.

        - Why communication protocols are necessary.

        - Why some applications require reliable delivery.

        - Why DNS and DHCP exist.

        - Why network security and troubleshooting are necessary.

  The objective is not to memorize these requirements. It is to understand the reasoning that makes each one necessary.

## 2. Problem One: How Can information Physically Travel?

2.1 The Probelm
   
   Imagine two independent computers:

    Computer A                     Computer B
      
    Application                      Application
        |                                 |
       Data                             Data
  
  Computer A contains information that Computer B needs. 

  However, the information exists inside computer A's computing environment. 

  Computer B cannot access that information automatically.

  Questions: How can information travel from one physical system to another?

     The computers require the mechanism that carries information between them.