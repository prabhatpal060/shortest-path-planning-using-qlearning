## Project Title:
**Obstacle Avoidance Path Planning Using Q-Learning Algorithm**

---

## Abstract:
This project presents an approach to solving obstacle avoidance and optimal path planning using reinforcement learning, specifically the Q-Learning algorithm. A matrix-based environment is provided via Excel input, where obstacles, paths, start, and goal points are marked. The system trains an agent to find the shortest path from the start to the goal while avoiding obstacles. It also visualizes the learned path using Python’s matplotlib library.

---

## Objectives:
- Implement Q-Learning for path planning.
- Avoid obstacles while finding the shortest path.
- Visualize the learning process and final path.
- Use real-time matrix input from an Excel file.

---

## Tools and Technologies Used:
- **Programming Language:** Python
- **Libraries:** NumPy, Pandas, Matplotlib, OpenPyXL
- **Platform:** Jupyter Notebook / Python 3.x
- **Input Format:** Excel Spreadsheet

---

## How the Code Works:
1. **Matrix Input:** The user provides an Excel file containing a grid matrix with different cell values:
   - `0`: Obstacle
   - `1`: Free path
   - `2`: Goal
   - `3`: Start

2. **Q-Learning Algorithm:** The code applies the Q-Learning algorithm with exploration and exploitation to find the optimal path.

3. **Path Extraction:** Based on the Q-values learned, the best path from the start to the goal is extracted.

4. **Animation:** The path is animated using matplotlib to demonstrate the agent's movement.

---

## Installation Steps:

1. **Clone the Repository**:
```bash
git clone https://github.com/prabhatpal060/shortest-path-planning-using-qlearning.git
cd yourrepository
```

2. **Install Dependencies**:
```bash
pip install -r requirements.txt
```

3. **Run the Project**:
```bash
python shortest_path.py
```

---

## Input Format:
- **Excel (.xlsx)** file with matrix layout
- Sheet name must be provided when running the script

Example matrix values:
```
0 = Obstacle
1 = Path
2 = Goal
3 = Start
```

---

## Sample Output:
- Console outputs the steps taken and reward value at each frame
- Visual animation of path from Start to Goal avoiding obstacles

---

## Result:
The system successfully identifies the shortest path between the defined start and goal points by avoiding obstacles and learning via Q-Learning.

---

## Future Scope:
- Integrate with real-time robotic movement
- Expand to 3D environments
- Add multiple goal-point handling and real-time learning
