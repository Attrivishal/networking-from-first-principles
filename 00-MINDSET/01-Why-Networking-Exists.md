So Guys MY name is Vishal Attri. And by the help of this repository i will try to explain you the fundamentals of the Networking. Because Networking plays a most important role in evey field. You can see that every device is connedted communicating sending data from one location to another and many more is only possible with the help of networking. 

So i request you to pleasr follow this journey with me. I will try to give my best to explain you in better and easy way. 


     ------->(: let's start with a beautifull smile :)<--------



Before going forward we need to set our mindset that every things around us is a network and try to think how they working,connected with each others. 


 ## Why Networking Exists?
 1. This is the fundamental Question?

  Before Learning IP address, MAC address, switches, Routers, TCP, DNS, or any other networking technology, we need to answer a much simple question: 

     Why does computer networking exists? 
      
      So, basically we all know that whenever any two computers want to communicate with each other or sending some information they must have to connected with each other. 

      Technically, When computer need to exchange information with other computer and systems. 
     
      A computer can process information locally, But many useful tasks require information that exists somewhere else. 

      For example:
      -> A browser need information from a web server. 
      -> An Application needs data from database. 
      -> A developer needs to connect with a remote server.
      -> A cloud server need to communicate with another cloud server. 

      All of these activites require communication. 
     
     Therefore networking exists because. 
        
         "Independent computing systems need a mechanism to exchnage information."

2. Okay, Let me start with the simplest Possible Problem. 
  
   Imagine you have a two computers: 

      COMPUTER A                           COMPUTER B 
         
         CPU                                  CPU


         MEMORY                              MEMORY 
 
   
    Computer A has some information:
    "HELLO"

    Computer B need to receive it

    The first Question that should come in your mind that how does that possible the information of Computer A send to Computer B Physically. 
     

     So computer can think the information from one computer to another. 


     Some form of communication medium  is required in this case: 

     For example:
         
              Computer A
                  |
                  |
            Communication Medium 
                  |
                  |
               Computer B
      
      But, There is a twist also what type of communication medium is required to send the information from "A -> B" and "B -> A".

      There should be some communicatio medium, Like when you want to travel from "Delhi -> Mumbai" Your communication medium can be Bus, Train Or Flight.
      
      So likewise in networking world we also do have some comunication medium in the form of:

         1. Copper cable
         2. Fiber-optic cable
         3. Radio waves
         4. Wi-Fi
         5. Cellular communication 
         6. Other physical or wireless technologies

      
   So this gives us our first fundamental requirement: 
     
        "Computers need a communication medium through which information can  travel."
    
3. But a Medium Alone is Not Enough
   
   Suppose we connect two computers with a cable: 

   A ------------- B

   Can they communicate Automatically?

    Not Necessarily. 

     Because computers still needs a way to represent the information being transmitted. 



    I hope you know this, that computers Ultimately Operates using Binary Information: 

        0  1
    
    Therefore,The information must be represented as signals that can travle through the communication medium. 

       Conceptually: 
         
         Application Data
                |
         Binary Information
                |
             Signals
                |
         Binary Information
                |
             Signals
                |
         Application data

  Now this creates another requirements:
     
        "Networking needs rules for representing and transmitting information."
    
This is where protocols and communication standards eventually become necessary. 


4. Now we facing the next problem, Who is the inforamtion For? 
   
   Like you can see slowly slwoly we are encountring the new challemges as move further. 

   Now imagine instead of two computers. We have severall :
    
    Computer: 
          A
          B
          C
          D
          E

    And Computer A wants to send "Hello" to Computer E. 

    Here, Now a new problem appears. 
       
        How does the network knows which computer should receive the information? 
   
    The network needs some way to indentify the intended destination that where the information should send on the correct location. 

     Conceptually: 

        Sender
          |
          | -- Send this info to "E"
         Network 
          |
          | -- B
          | -- C
          | -- D
          | -- E <-- Destination 
    
    So, Here we encounter a new concept "ADDRESSING" 
     
     Now let me tell you what is  ADDRESSING ?

        Imagine you're in a large office building. You want to send a letter to your friend E who works on the 4th floor. 
          
        And you drop a letter at the front desk and say :

          "Please deliver this To E."

        But wait, here is the twist , there are three people named E in the building.      

         1. E in Accounting (Floor 2)
         2. E in Marketting (Floor 4)
         3. E in Engineering (Floor 7)

         The front desk ask: "Which E?"

         So here you need to be more specefic. You need to give an full address. 

    What Is addressing?
        
        "Addressing is a simple way to uniquely identify something so information can reach to the right place."
    
    Think of it like: 

         Real world                       Networking world

         House Address                      IP address
         Appartment Number                  Port number
         Person's Name                      Hostname(eg. Google.com)
         Building Name                      MAC address (hardware address)

5. Why Isn't One Address Enough?
    
    At, First it may seem that every computet could simply have one uinque address. 
   
   But consider a larger system. 
      
        Computer A
           | -- Browser
           | -- SSH Client
           | -- Email Client
           | -- Other Applications
      
      Suppose Computer A recieves some network traffic. 
        
           The computer knows:
                  "This traffic is intended for me."
      But another questions remains. 
        
           Which application on this computer should receive it? 
      
   So bacisally one address is not enough for sending the data correctly.

   Because :
      
        A computer can have many  application running at the same time, and the network needs to know which one should reveive the incoming data. 


   