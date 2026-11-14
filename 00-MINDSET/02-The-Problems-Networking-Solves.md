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

     That mechanism involves a transmission medium and the technology needed to transmit and receive signals through it.

     Examples include:

      1. Copper Ethernet cables.
      2. Fiber-optic cables.
      3. Radio waves used by Wi-Fi.
      4. Cellular radio networks.

      The precise transmission method depends on the technology being used. 

## 2.2 Why this problem exists
   
   Computers process information internally, but communication  between separate systems requires information to cross a physical or wireless boundary.

   The sender nust reprsent information in a form suitable for transmission. The receiver must be able to recover and interpret that information.

   A cable  alone does not gurantee sucessful communication. The devices also need compatible interfaces, signalling methods, and communication rules. 

## 2.3 The resulting  requirement 
    
     Requirement: 
        
        A networking system needs a transimission mechanism that allows information to travel between systems.

     This leads us toward the physical layer, signaling, network interfaces,and transmission media. 

## 2.4 Defend your answer
    
    Questions: Why do computers  needs a communication medium?
   
   A strong 
    







