

# 🐍 Deep Q-Learning Snake Game

This project is an AI-based Snake game where the agent learns to play using **Deep Q-Learning** (DQL). Built with **PyTorch** and **Pygame**, the agent is trained using reinforcement learning to maximize its score by learning optimal actions based on its environment.  

---

## 🚀 Features

- ✅ Implementation of Deep Q-Learning from scratch
- 🎮 Real-time Snake gameplay with Pygame
- 📊 Training visualization: scores, mean scores, and game performance
- 💾 Experience Replay Buffer and Epsilon-Greedy Policy
- 🧠 Neural Network as the function approximator for Q-values
- 🔁 Continuous training with saving of best models

---

## 🧠 How It Works

The agent is trained using the **Deep Q-Learning algorithm**:

1. **State Representation**:  
   The environment is observed as a state vector with information about obstacles, food location, and current direction.

2. **Action Space**:  
   Actions are encoded as `[straight, right, left]` for simplicity.

3. **Reward Function**:  
   - +10 for eating food  
   - -10 for dying  
   - 0 for every other step

4. **Neural Network (DQN)**:  
   A fully connected model predicts Q-values for each possible action.

5. **Epsilon-Greedy Policy**:  
   Used for exploration vs. exploitation during training.

6. **Experience Replay**:  
   Stores game experiences to break correlation and improve learning.

---

## 📂 Project Structure

 -├── agent.py # Contains the DQN agent logic and training
 -├── model.py # Neural network architecture 
 -├── game.py # Game environment using Pygame  
 -├── helper.py # Real-time plot of score trends 
 -├── model.pth # Saved model (optional) 
 -├── requirements.txt # Python dependencies 
 -└── snake_game_human.py # game where a human player can control the snake using the keyboard 
 -└── README.md # Project overview

---

## 🖥️ Demo

<p align="center">
  <img src="https://media.giphy.com/media/Jo5Dcdh8yFi4sE0M7s/giphy.gif" width="400" />
</p>

---

## ⚙️ Requirements

Main Libraries:

Python 3.7+

PyTorch

Pygame

Matplotlib

---

## 📈 Output

Real-time game window with Snake and food.

Live plot showing score and mean score over time.

Model saved when best performance is achieved.

---

## 📚 Concepts Used

Reinforcement Learning

Deep Q-Networks (DQN)

Epsilon-Greedy Exploration

Neural Networks

Experience Replay

Temporal Difference Learning

---

## 🏆 Results

After training for ~500-1000 games, the agent significantly improves and learns to avoid collisions and chase food effectively. You can tune parameters in agent.py and model.py for better performance.

---

## 📌 Future Improvements

Implement Double DQN

Add Prioritized Experience Replay

Switch to CNN-based state input (grid representation)

Save game replays as GIFs or videos

---

## 🤝 Contributing

Pull requests and issues are welcome! If you’d like to enhance this project or fix bugs, feel free to fork and contribute.

---

## Made with ❤️ by Shrestha!



