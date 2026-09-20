# Activity 5: The Whispering Cave — DFS Adventure
## Sessions 10, 11, 12
## Due date: 09/20/2026
## ADRIANA ROSALES GONZÁLEZ
## Delivery Format: Video URL + Markdown file

---

## 1. Search Space (Session 11)

- **Initial State:** Entrance  
- **Goal State:** Treasure Room  
- **Total Paths:**

  <img width="626" height="592" alt="image" src="https://github.com/user-attachments/assets/62034563-fc10-48a6-9d0e-c9b7539fdb92" />


**Comment:** This shows the entire search space and how many possible paths exist from the Entrance to the Treasure Room.

---

## 2. Tunnel Rules (Session 10)

- **Query 1:**
<img width="623" height="611" alt="image" src="https://github.com/user-attachments/assets/2c2db36d-4c36-4969-8abc-a51d645a8325" />

- **Query 2:** 
<img width="554" height="345" alt="image" src="https://github.com/user-attachments/assets/cb75b1c1-0583-439e-817b-bd8f8bd4a3a7" />

**Comment:** The trace demonstrates how the recursive rule `reachable(X, Y)` goes deeper tunnel by tunnel until the destination is found.

---

## 3. Depth-First Explorer (Session 12)

- **Full traversal order:** [write here the exact order of chambers visited]  
- **Dead-end chamber visited:** [name of the chamber]  

<img width="565" height="524" alt="image" src="https://github.com/user-attachments/assets/f2b5d95d-589c-4c6b-a5b5-640796a981a3" />


**Comment:** At the dead end, DFS had no new moves and had to backtrack. The final screenshot shows the path taken and the total step count.

---

## 4. Reflection (A5_ReflectionQuestions.md)

1. What is a stack and why does DFS use it?
A stack is like a pile of plates: the last one you put on top is the first one you take off (LIFO — last in, first out). DFS uses a stack because it always wants to go deeper into the cave before coming back. Each new chamber is added on top, and when DFS can’t go further, it removes the top chamber to backtrack.

2. Why is the visited list important?
The visited list keeps track of which chambers have already been explored. Without it, DFS would get stuck in loops forever (for example, the Torch Hallway → Echo Chamber → Bat Roost → Entrance cycle). By remembering visited chambers, DFS avoids repeating the same path and can eventually reach the treasure.

3. Was the path DFS found the shortest possible path?
No, DFS does not guarantee the shortest path. It only guarantees that it will eventually find a path to the goal. In the app, the Search Space tab shows all possible paths, including shorter ones. The path DFS actually walked was longer than the shortest possible path, which proves DFS is about exploration, not efficiency.

4. Personal takeaway
This activity helped me understand how DFS works step by step. I saw how the stack controls the order of exploration, how backtracking happens at dead ends, and why the visited list is essential. It showed me that DFS is powerful for exploring all possibilities, but if I need the shortest path, I would use a different algorithm like Breadth‑First Search.


---

- Video link/file: https://youtu.be/n7z1_wZhsxI



## 📂 Evidence

- `Step1_SearchSpace.png`  
- `Step2_TunnelRules.png`  
- `Step3_DeadEnd.png`  
- `Step4_Final.png`  
- `A5_ReflectionQuestions.md`  
