![PyroDeck Logo with Icon](https://github.com/ckfast/PyroDeck/blob/4ee63fe5b90d5df9740ecbb86bdcbd6d85212fa9/images/PyroDeckBanner.png)

# What is PyroDeck?
PyroDeck is an open source project with one goal in mind: Have a way to ignite fireworks safely from a distance, and in a way that is easy, fun, and of course, really cool. 

There are 2 main parts of the PyroDeck system, the **Master Control**, and the **Nodes**. In a really short paragraphs, here is what each of them do.

### Master Control
The **Master Control** panel does exactly what the name says. It tells the system what to do. Based on manual or automated controls, it sends out commands (with RS485 JSON messages) to the nodes in the system. These commands can be launch commands, or query commands to recieve the status of the nodes. 

The **Master Control** panel has different opperating modes which include fully manual control over every channel, and automatic control that runs through a cue list to launch one or more fireworks at a time. It is also possible to have a "wait for input" cue to wait for a button to be pressed before carrying on with the cue list. I plan to include more features with both opperating modes as time comes.

### Nodes
The **Nodes** are the "workmen" of the system. They are up close to the danger and send the signals to ignite the fireworks. They recieve the commands given by the Master Controller and follow what it says, whether it be to ignite a firework, or respond with the status of each port. 

The **Nodes** have a 3 digit address which is how the Master Control identifies each node. With each command sent, there is a specific address in which the Node checks for. If the address matches it reads the command, if not it discards the message and watches for other commands. 

# Todo List
### Node
- [x] Develope the Node's Relay PCB Module
- [x] Develope the Node's UI PCB Module 
- [ ] Develope the Node's MCU PCB Module
- [ ] Finish Developement of the Node's code.

### Master Control
- [ ] Literally Everything


![PyroDeck Icon](https://github.com/ckfast/PyroDeck/blob/8be9890bc0634977935303a31299fa7303ae7cae/images/PyroDeckLogoSmall.png)
