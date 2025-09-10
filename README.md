# 🚀 Deep Q-Learning - Lunar Lander

This project demonstrates how I successfully programmed a spacecraft to land safely on the surface of the moon without crashing, using **Reinforcement Learning** and **Neural Networks**.

---

## 🌌 Mission Description
The objective was to build an agent capable of controlling a lunar lander in a physics-based simulation. The challenge lies in ensuring that the lander reaches the landing zone gently, without crashing, by learning from trial and error.

To achieve this, I used the `LunarLander-v2` environment from OpenAI Gym. The environment provides continuous state observations (position, velocity, angle, etc.) and a set of discrete actions (engines to fire). The agent must learn how to balance and descend safely.

---

## 🤖 How the Agent Learns
I implemented the **Deep Q-Learning (DQN)** algorithm, a type of Reinforcement Learning technique that combines Q-Learning with a deep neural network.

### Key Components:
- **Agent:** Learns which action to take given the current state.
- **Neural Network:** Approximates the Q-value function that predicts future rewards.
- **Replay Buffer:** Stores past experiences to train the network using randomized samples.
- **Target Network:** A copy of the Q-network used for stable learning.
- **Reward Function:** Encourages successful landing and penalizes crashing or going off course.

During training, the agent explores different actions and gradually learns the best strategies to land safely through rewards and penalties.

---

## 🧠 Technologies & Concepts Used
- Deep Q-Learning (DQN)
- OpenAI Gym (`LunarLander-v2`)
- Experience Replay
- Target Network
- TensorFlow (for building and training the neural network)
- Numpy, Python Standard Libraries

---

## 💻 Running the Project
Make sure you have the required libraries:

```bash
pip install gym==0.24.0 tensorflow numpy Pillow
```

Then run the notebook:
```bash
jupyter notebook Deep_Q_Learning_Lunar_Lander_GitHub_Version.ipynb
```

---

## 📈 Training Summary
The agent starts with random actions, receiving low rewards or penalties for crashing. Over time, as it learns from experience, it develops a reliable strategy for soft landings. After training, the lander consistently performs safe landings.

---

## 🚀 Results
- The lander successfully learns to balance, reduce speed, and land precisely.
- The average reward increases steadily over episodes.
- The trained agent can be tested on new episodes with high success.

---

## 🔭 Future Work
- Integrate Double DQN for better stability.
- Try Prioritized Experience Replay.
- Convert to a script with CLI arguments.
- Visualize metrics with TensorBoard.

---

## 👨‍💻 Created by
**Abdallah A. M. Iqelan**


