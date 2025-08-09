# ♗♞ Reinforcement Learning Pathfinding: Bishop vs Knight

## 📌 Project Summary
This project demonstrates the application of **Q-Learning** to a game-inspired pathfinding problem on a chessboard-like grid.  
Two different agents — a **Bishop** and a **Knight** — are trained to navigate a 5×5 board and reach a goal position, each using their own movement rules.

The aim is to compare:
- Learning dynamics
- Efficiency of movement strategies
- Reward optimization over training episodes

The project can serve as:
- An **educational example** of Reinforcement Learning (RL)
- A **data-driven experiment** comparing different action spaces
- A **visual tool** to explain RL concepts to non-technical audiences

---

## 🎯 Business & Analytical Value
While this problem is framed as a chessboard game, the methodology applies to **real-world routing and decision-making tasks**, such as:
- **Logistics**: Optimal route finding with different vehicle capabilities
- **Robotics**: Movement planning with mobility constraints
- **Operations Research**: Pathfinding in constrained environments

Key **data analytics aspects**:
- Tracking and visualizing reward trends
- Comparing efficiency metrics between agents
- Evaluating convergence speed in Q-Learning

---

## 🔍 Methodology
**1. Problem Setup**
- Board size: `5x5`
- Goal position: `(4, 0)`
- Agents:
  - **Bishop**: moves diagonally
  - **Knight**: moves in L-shapes

**2. Q-Learning Parameters**
- Episodes: `1000`
- Learning rate (α): `0.1`
- Discount factor (γ): `0.9`
- Exploration rate (ε): `0.1`

**3. Metrics Tracked**
- **Total reward per episode** — learning progress
- **Path length to goal** — efficiency
- **Convergence rate** — training stability

---

## 📊 Key Insights
- **Bishop** learns faster when the goal is positioned diagonally reachable within fewer moves.
- **Knight** takes longer to converge due to a more complex movement pattern but shows better adaptability in certain layouts.
- Reward curves show clear improvement after ~200 episodes for both agents, indicating stable learning.

---

## 📈 Visualizations
### Reward Progress Over Time
Shows how cumulative rewards evolve during training, illustrating learning speed and stability.

![Reward Trends](docs/reward_trends.png)

### Agent Path Visualization
Example of a learned path for Bishop:
♗ → ♗ → ♗ → ✔

yaml
Копировать
Редактировать
Each step is rendered on a chessboard grid with move-by-move visualization.

---

## 🛠 Tech Stack
- **Python 3.10+**
- **NumPy** — numerical computations
- **Matplotlib** — data visualization
- **IPython** — output handling
- **time** — animation delays

---

## 📂 Project Structure
├── rl_pathfinding.py # Main Q-Learning implementation
├── docs/
│ ├── reward_trends.png # Reward plot
│ └── example_path.gif # Path animation
├── README.md # Project documentation

yaml
Копировать
Редактировать

---

## ⚙️ How to Run
```bash
git clone https://github.com/yourusername/rl-pathfinding.git
cd rl-pathfinding
pip install -r requirements.txt
python rl_pathfinding.py
📌 Potential Extensions
Experiment with larger boards or different goal positions

Add obstacles to test adaptive pathfinding

Implement SARSA or Deep Q-Learning for comparison

Track exploration vs exploitation ratios
