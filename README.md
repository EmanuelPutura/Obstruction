# Obstruction
 Obstruction is a 2D game written in Python, in which players take turns in marking squares on a grid. The first player unable to move loses.
 The game is played between the user and the computer. The AI is implemented using the minimax algorithm.
 
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
 For the UI, the options are ```gui``` and ```console```. The strategy can be ```beginner```, ```random``` or ```minimax``` and the human/computer symbol can be ```X``` or  ```O```. Also note that for the second player symbol the letter 'O' is used instead of '0', because of displaying considerations.
 
 
 ## Features
 1. Console User Interface
 2. Graphical User Interface, built with the Tkinter framework
 3. AI - implemented using the MiniMax Algorithm
 4. UnitTesting (testing most of the basic functionalities)
 5. Layered Arhitecture
 6. Code commentaries for almost all the functions and classes
 7. Multiple available strategies to be used by the computer player


 ## AI Implementation Description
 The AI analyses every possible move from the current board state by using a minimax evaluation function and it tries to maximize the score of the move if it's the computer's turn, or minimize it if it's the user's turn (the AI thinks 2 moves in advance, more than that would seriously affect the time performance). Hence, it decides which move is the most profitable, taking into consideration the current game state.
