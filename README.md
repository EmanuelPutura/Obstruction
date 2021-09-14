# Obstruction
 Obstruction is a 2D game written in Python, in which players take turns in marking squares on a grid. The first player unable to move loses.
 
 <p align="center"> <img src="https://github.com/EmanuelPutura/Obstruction/blob/main/img/game.png" height="400"/> </p>
 
 
 ## Setup
 1. Clone the repo:
    ```sh
    $ git clone https://github.com/EmanuelPutura/Obstruction
    ```
 2. Install project dependencies:
    ```sh
    $ pip install jproperties
    $ pip install texttable
    ```
 3. From the project's location:
    ```sh
    $ cd ./src
    $ python main.py
    ```


 ## Usage
 The users can change the game settings before launching the game (e.g., the user can choose between a console-based UI or a graphical UI, the AI strategy, the user's and the computer's board symbols). This can be done by modifying the ```settings.properties``` file (located in the ```src``` folder of the project). The default game settings are:
 ```sh
 ui = gui
 strategy = minimax
 human_symbol = X
 computer_symbol = O
 ```
 For the UI, the options are ```gui``` and ```console```. The strategy can be ```beginner```, ```random``` or ```minimax``` and the human/computer symbol can be ```X``` or ```O```. Also note that for the second player symbol the letter 'O' is used instead of '0', because of displaying considerations.
 
 
