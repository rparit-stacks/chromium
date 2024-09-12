### **Project Objective**
The primary objective of this project is to develop an engaging, interactive, and user-friendly Tic Tac Toe game for Android devices. The app is designed to offer an enjoyable and intuitive gaming experience with a classic appeal, aiming to recreate the timeless fun of Tic Tac Toe in a modern digital format. The app allows users to play against another player or an AI opponent, with features that enhance gameplay through responsive feedback, visual appeal, and smooth interactions. The goal is to provide a platform where players can enjoy quick, casual gaming sessions, making the app a go-to option for relaxation and entertainment.

### **Introduction**
Tic Tac Toe, also known as Noughts and Crosses, is a classic pen-and-paper game that has been enjoyed for generations. It involves two players taking turns to mark the spaces in a 3x3 grid with their respective symbols, X or O. The winner is the first player to align three of their marks horizontally, vertically, or diagonally. The simplicity of the game combined with its strategic elements makes it popular among all age groups, from children to adults.

This project aims to bring the classic game to mobile devices, allowing users to enjoy it anytime and anywhere with the convenience of a smartphone. The Tic Tac Toe app is built on the Android platform using Java for game logic and XML for layout design, ensuring compatibility across a wide range of devices. The app incorporates a blend of modern design principles and traditional gameplay mechanics, creating a seamless experience that is both nostalgic and refreshing.

### **Key Features of the App**:
1. **User-Friendly Interface**: 
   - The app is designed with simplicity and accessibility in mind, featuring a clean and minimalistic UI that enhances the overall user experience. The interface uses clear symbols and intuitive controls, making it easy for players of all ages to engage with the game.

2. **Single and Multiplayer Modes**: 
   - Users have the flexibility to play against another person on the same device in the multiplayer mode or test their skills against the AI in the single-player mode. The AI opponent is programmed with varying levels of difficulty, providing both casual play and challenging experiences.

3. **Realistic Game Feedback**: 
   - The app includes tactile vibration feedback on each move, which adds to the immersion and makes the game feel more interactive. When a player wins, the game triggers a longer vibration, enhancing the sense of achievement.

4. **Score Tracking System**: 
   - The app keeps track of each player's scores, including wins, losses, and draws. This feature encourages competition, allowing users to monitor their performance over time. The scores are saved using SharedPreferences, ensuring data persistence even when the app is closed.

5. **Visually Appealing Design**: 
   - Incorporating a modern aesthetic inspired by neumorphic design principles, the app's visuals are both elegant and functional. The use of soft gradients, subtle shadows, and neumorphic buttons provides a sophisticated look while maintaining clarity and ease of use.

6. **Cross-Device Compatibility**: 
   - The app is optimized for various screen sizes, ensuring that the game looks and functions well on both phones and tablets. It is built with responsiveness in mind, offering consistent performance across different Android devices.

### **Technical Overview**:
- **Development Tools**: The app is developed in Android Studio, leveraging Java for backend logic and XML for UI design.
- **Core Logic**: The game logic is implemented using Java, handling player turns, checking for winning conditions, and managing game states.
- **Vibration and Feedback**: Vibration effects are managed using Android’s Vibrator class, providing immediate feedback with short and long pulses based on gameplay events.
- **Data Management**: Player scores are managed using SharedPreferences, which allows the app to store and retrieve game data efficiently, ensuring scores are persistent between sessions.

### **Conclusion**:
This Tic Tac Toe app is designed to provide a quick, engaging, and satisfying gameplay experience that appeals to casual gamers. With its modern design, smooth performance, and responsive feedback, the app aims to revive the charm of a traditional game with the convenience of digital play. Future enhancements may include additional modes, customizable themes, and online multiplayer capabilities, expanding the app's reach and functionality.

---

# Block Diagram
![image](https://github.com/user-attachments/assets/caa64e2d-544d-4276-9048-ca523653e947)

The block diagram of the Tic Tac Toe game app visually represents the key components and their interactions within the application. Each block signifies a major part of the system, highlighting how the game's core functionalities are structured and interlinked.

#### **Components of the Block Diagram:**

1. **User Input (Taps/Clicks)**
   - **Description**: This block represents the input actions from the players, such as tapping or clicking on the game board to make a move.
   - **Functionality**: It captures the player's move and sends it to the game logic for processing.

2. **Game Logic (Handles Moves, Win Conditions)**
   - **Description**: This is the core processing unit of the game, responsible for managing moves, checking for win conditions, and updating the game state.
   - **Functionality**: It validates each move, updates the board state, and checks whether any player has won, lost, or if the game is a draw.

3. **Vibration System (Feedback on Moves)**
   - **Description**: This component provides haptic feedback to the players after each move, enhancing the user experience with physical vibrations.
   - **Functionality**: It triggers short vibrations for regular moves and longer vibrations for winning or losing scenarios.

4. **UI Components (Board, Scores, Status Display)**
   - **Description**: This block covers the visual elements of the game, including the Tic Tac Toe grid, score display, and status messages (e.g., whose turn it is).
   - **Functionality**: It updates the display according to the game state, showing moves on the grid, current scores, and game status messages.

5. **Score Storage (SharedPreferences)**
   - **Description**: This component handles the storage of players' scores using the device’s local storage, specifically SharedPreferences.
   - **Functionality**: It keeps track of the scores between game sessions, allowing players to see their progress over time.

#### **Overall Workflow:**
- Players interact with the app through taps and clicks, which are processed by the Game Logic.
- The Game Logic updates the game state based on the moves, checks for win conditions, and communicates with the UI Components to update the display.
- Vibration feedback is provided after each move to enhance the player's engagement.
- Scores are updated and stored in the Score Storage component, ensuring continuity between sessions.

### **Purpose of the Block Diagram:**
The block diagram provides a clear overview of the system’s architecture, showing how user actions are processed and reflected in the game. It helps developers understand the flow of data and the interaction between different components, ensuring that each part functions cohesively within the overall system.


# UseCase Diagram
![Untitled (8)](https://github.com/user-attachments/assets/9e92c29c-046a-407c-9d45-38753bc80eb8)
The use case diagram of the Tic Tac Toe game app illustrates the interactions between the users (players) and the system’s various functionalities. It highlights the primary actions that can be performed within the app, demonstrating the roles of the players and the system’s responses.

#### **Components of the Use Case Diagram:**

1. **Actors:**
   - **Player 1 and Player 2**: Represent the two participants who interact with the game. These actors are involved in starting the game, making moves, and interacting with the game system through the app interface.

2. **Use Cases:**
   - **Start Game**:
     - **Description**: This use case allows players to initiate a new game session. It resets the board, scores, and sets the game status to active.
     - **Interactions**: Both Player 1 and Player 2 can trigger this action to begin a new match.

   - **Make a Move**:
     - **Description**: Represents the core gameplay action where a player makes a move by tapping on a grid cell.
     - **Interactions**: Both players alternate making moves until a win condition or draw is achieved.

   - **Check Win Conditions**:
     - **Description**: The system automatically checks the board after each move to determine if there is a winner or if the game ends in a draw.
     - **Interactions**: This is a system-triggered action that responds to each player’s move.

   - **Update Game Status**:
     - **Description**: Updates the game’s current status, such as displaying which player's turn it is, declaring a winner, or showing a draw.
     - **Interactions**: This use case is managed by the system and displayed on the screen for both players.

   - **Display Scores**:
     - **Description**: Shows the current scores of both players, updating after each game session.
     - **Interactions**: The system maintains and updates this display after each game concludes.

   - **Exit Game**:
     - **Description**: Allows players to exit the current game session and return to the main menu or quit the app.
     - **Interactions**: Both players can use this option to terminate the session at any time.

   - **Provide Vibration Feedback**:
     - **Description**: Enhances the gameplay experience by providing tactile feedback when a player makes a move or when the game concludes.
     - **Interactions**: Triggered automatically by the system in response to game actions.

3. **Relationships:**
   - **Player Interactions**: Both players interact with the core functionalities such as making moves, starting the game, and exiting.
   - **System Responses**: The system manages feedback mechanisms such as checking win conditions, updating the status, displaying scores, and providing vibration feedback.

#### **Purpose of the Use Case Diagram:**
- The use case diagram provides a high-level view of how the Tic Tac Toe game functions from the user's perspective. It helps developers and stakeholders understand the primary interactions within the app, ensuring that all expected functionalities are accounted for during development.
- It serves as a blueprint for building user-centric features, enhancing the app’s usability, and ensuring a seamless player experience.



# DFD
![image](https://github.com/user-attachments/assets/5a27f463-454e-4395-af2c-26aa4a324ce6)

The Data Flow Diagram (DFD) of the Tic Tac Toe game app illustrates the flow of data within the system, highlighting how information moves between the various components and processes. The DFD provides a clear representation of how user inputs are handled, processed, and outputted, ensuring a smooth functioning of the game.

#### **Components of the Data Flow Diagram:**

1. **External Entities:**
   - **Player 1 and Player 2**:
     - **Description**: These entities represent the users interacting with the game. They provide inputs in the form of moves and receive outputs such as game status updates, vibration feedback, and scores.

2. **Processes:**
   - **1.0 Start Game**:
     - **Description**: This process is triggered when the players choose to start a new game session. It initializes the game board, resets scores, and sets the game status to active.
     - **Data Flow**: Receives a start command from the players and sends a reset signal to the game board.

   - **2.0 Make a Move**:
     - **Description**: Handles the player's actions when they make a move by tapping on the game grid. It captures the input and sends it to the game logic.
     - **Data Flow**: Receives player input (move) and updates the game state accordingly.

   - **3.0 Check Win Conditions**:
     - **Description**: After each move, this process evaluates the current state of the board to check if a winning condition is met or if the game has ended in a draw.
     - **Data Flow**: Takes the updated game state from the previous process and determines the outcome.

   - **4.0 Update Game Status**:
     - **Description**: Updates the status display for the players, showing whose turn it is, who won, or if the game is a draw.
     - **Data Flow**: Receives results from the win-check process and updates the display.

   - **5.0 Display Scores**:
     - **Description**: Manages the score display, showing the current scores of Player 1 and Player 2.
     - **Data Flow**: Updates scores based on the results of each game session and sends this data to the display.

   - **6.0 Provide Vibration Feedback**:
     - **Description**: Provides tactile feedback in the form of vibrations when moves are made or when the game concludes.
     - **Data Flow**: Receives signals based on game events and triggers vibrations.

   - **7.0 Exit Game**:
     - **Description**: Allows players to exit the current game session and return to the main menu or quit the app.
     - **Data Flow**: Receives an exit command from the players and stops the game processes.

3. **Data Stores:**
   - **D1: Game State**:
     - **Description**: Stores the current state of the game, including player positions on the grid and game status.
     - **Interactions**: Updated after each move and referenced when checking win conditions.

   - **D2: Player Scores**:
     - **Description**: Maintains the scores of both players across game sessions.
     - **Interactions**: Updated after each game session and displayed to the players.

4. **Data Flows:**
   - **Player Input to Make a Move**: Data flows from the players to the process that handles their moves.
   - **Game State Updates**: Moves data between the processes to maintain the current state and status of the game.
   - **Score Updates**: Data flows from game processes to the score display component to keep the scores current.
   - **Vibration Feedback**: Data flows from the system to provide physical feedback based on game events.

#### **Purpose of the Data Flow Diagram:**
- The DFD provides a detailed overview of how data moves within the Tic Tac Toe game app. It helps developers understand the internal workflow of the system, ensuring that each component receives and processes data correctly.
- It highlights the interactions between user actions and system responses, ensuring that the data architecture is efficient and logically structured.

