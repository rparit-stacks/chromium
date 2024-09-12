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

# DFD
![image](https://github.com/user-attachments/assets/5a27f463-454e-4395-af2c-26aa4a324ce6)
