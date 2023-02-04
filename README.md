# Digital Judge for Party Game “Werewolf”
#### Inventors:
#### Yue Feng, Weicheng Huang, May 2016
#### Registered Patent: https://patents.google.com/patent/CN206642349U/

### Background:
##### The werewolf game is a strategy-based tabletop game that involves multiple players. The game is driven by language description and tests the players' verbal skills and analytical abilities. On average, it requires 8 to 16 players to participate and a dedicated host to keep track of the game events and ensure a smooth progression.
##### Traditionally, the game is played in a face-to-face setting, but this approach often faces several challenges such as a shortage of players, lack of willingness among players to serve as the host, absence of a reliable scoring system to reflect the players' levels, and difficulty in classifying players based on their skills and location, which can discourage beginner players.
##### Therefore, we introduce an online and offline integrated werewolf game system, which is part of the gaming systems domain. The system consists of a game server, a web server, and a terminal gaming device that is connected via a wired or wireless network. The game server handles the logical operations of the werewolf game, while the web server manages the backend, data management, authorization, and identity management of the game. The terminal gaming device interacts with players by exchanging input and output data. The newly introduced werewolf game system offers a convenient solution for tabletop bars and operating companies through its seamless integration of online and offline experiences. It also enhances the overall user experience and helps form a social community around the werewolf game.

### Technical Scheme:
![alt text](https://github.com/ttopeor/Werewolf/blob/main/overall.PNG)
##### As the graph shown above, our gaming system consists of game servers, web servers, and terminal gaming machines that are connected to the network via wired or wireless means. The game server is responsible for conducting the logic operations of the Werewolf game, managing the output data of the terminal gaming machines, and collecting input data from them. The web server handles the backend administration, data management, authorization management, and identity management of the Werewolf game. It gathers player data from the game server and oversees its operation status. The terminal gaming machine facilitates input and output data interaction between the players and the Werewolf game and is controlled by both the game server and the web server.
##### The game server comprises of a game process management unit and multiple game process units. The multiple game process units are controlled by the game process management unit, and both the game process management unit and the multiple game process units communicate with the client’s main process within the terminal gaming machine to exchange data.
##### A web server includes a terminal management system, a game management system, a web management system, and a backend machine management system. The terminal management system is used to control maintenance, freeze, activation, and firmware updates of the terminal game machine. The game management system is used to control the game start and stop permission, change game options, and identify player identity. The web management system is used to manage the Werewolf game website, forum, and score query. The backend machine management system is used for data statistics, billing, and score management. The terminal management system interacts with the terminal game machine, the game management system interacts with the game server, the web management system interacts with the game website client, and the backend machine management system interacts with the terminal backend machine used for the game backend management.
##### The web management system includes a query system, a forum system, and an official website. The query system is used to inquire about player information and board game bar information. The forum system is used to publish information from the operating company, and collect feedback from board game bars and players, and the official website is used to display the download client for the Werewolf Game.
##### The back-end machine management system includes a data statistics system, a reservation system, and a billing system. The data statistics system is used to compile statistics on the number of players, cash flow, number of game sessions, and game results. The reservation system is used to manage player and board game bar reservations, and the billing system is used to charge players based on the usage of the game machine.
 
![alt text](https://github.com/ttopeor/Werewolf/blob/main/gametable.PNG)
##### The werewolf game system, as shown in the above figure, also includes a handle. The handle is electrically connected to the terminal game machine and communicates with the terminal game machine through the I2C communication method. The handle includes a central control chip, a OLED tiny display, a joystick, and light bulbs. The central control chip is located inside the handle's shell, and the OLED tiny display, joystick, and light bulbs are located on the handle's shell. The liquid crystal display, joystick, and light bulbs are all electrically connected to the central control chip. The game display data output by the central control chip is displayed through the OLED tiny display and light bulbs, and the player input data from the joystick is processed by the central control chip.
##### The terminal game machine includes a control module for running the client's main process, a power module, a WIFI module, an I2C module, a sound output module, and a handle power module. The I2C module is used for communication with the handle; the handle power module is used for supplying power to the handle; the WIFI module is used for wireless communication with the game server and the web server; the power module is used for supplying power to the handle; the sound output module is used for outputting audio; and the control module is used for controlling the input and output of the power module, the WIFI module, the I2C module, the sound output module, and the handle power module. The control module is electrically connected to the power module, the WIFI module, the I2C module, the sound output module, and the handle power module, and the sound output module is electrically connected to the speaker.

### Conclusion:
##### The present invention provides a Werewolf game system that integrates online and offline experiences. It consists of a game server, a web server, and terminal gaming machines, which can be connected to input/output devices such as controllers. The terminal gaming machines can communicate with the game server and web server, and through the input/output devices and terminal gaming machines, they can interact with the online server. This enables online and offline interaction and facilitates the management of tabletop bars and operating companies, enhancing the online and offline user experience. Additionally, it includes an online point management system, a fee system, a reservation system, etc., which enhances the convenience and stickiness of playing the Werewolf game.


### Prototype (2016):
![alt text](http://url/to/img.png)