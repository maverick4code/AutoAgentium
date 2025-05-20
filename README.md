# AutoAgentium

Welcome to **AutoAgentium**, my personal portfolio for building AI-powered multi‑agent workflows. Below you’ll find 5 bite‑sized subprojects, each one a mini project demonstrating a unique way to let these agents collaborate on real problems, from plotting stock charts to crafting full reports.

---

## 🔧 Subprojects

### 1. CodeAutomator

**Pattern:** Two‑Agent Code Flow

- Code Writer generates clean Python scripts.

- Executor runs those scripts locally and returns results.

- Demo: Fetched YTD(Year to Date) gains for NVDA & TSLA, plot with Matplotlib.

---

### 2. SequentialChain

**Pattern:** Step‑by‑Step Chat

Sometimes you need a clear sequence: “First fetch the data, then clean it, then visualize it.” **SequentialChain** does exactly that. I wired up agents so each one waits for the previous to finish before jumping in.

- Agents tackle subtasks in sequence.
  
- Adapted for customer service bots handling one query at a time.
 
**Use case:** Works for onboarding bots and multi‑stage data pipelines. 

---

### 3. NestedSquad

**Pattern:** Nested Chat Teams

In **NestedSquad**, a “manager” agent builds up a mini squad—each member with its own role and oversees their conversation.

**Use case:** I tested this by having the manager coordinate a mini newsroom: one agent researched topics, another drafted paragraphs, and a third did quick fact‑checks. It felt like running a tiny editorial team entirely within a chat session.

---

### 4. ToolboxFree

**Pattern:** Function Mode vs. Free‑form Code

Here I explored two styles:

* **Function Mode:** Agents call your pre‑written helper functions (e.g: `get_stock_data()` or `plot_chart()`). It makes scripts concise and predictable.
* **Free‑form Mode:** Agents are free to invent any code they need, loading libraries and writing new functions in the session.

**Lesson learned:** Function Mode gives you more control and safety, while Free‑form Mode unlocks maximum creativity.

---

### 5. StockPulseReport

**Pattern:** Group‑Chat Planning

Here, I assembled a squad of five agents—**Planner**, **Engineer**, **Executor**, **Writer**, and **Admin** and tasked them with generating a full stock‑performance report:

1. **Planner** breaks down “generate stock report” into steps.
2. **Engineer** wrote the Python code to crunch the data.
3. **Executor** ran the code and handed back charts and tables.
4. **Writer** added it all into a polished Markdown report.
5. **Admin** checked in at each milestone, asking for human approval when needed.

Output:  A full stock report—completely automated.

---

## ⚙️ Getting Started

1. **Clone** this repo:

   ```bash
   git clone https://github.com/maverick4code/AutoAgentium
   cd AutoAgentium
   ```
2. **Install** dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

If you have ideas to make this project better, want to collaborate, or just chat about AI automation, you can connect with me.
LinkedIn: https://www.linkedin.com/in/sagar-shahari-703b84257/
