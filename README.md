# AutoAgentium

Welcome to **AutoAgentium**, my personal portfolio for building AI-powered multi‑agent workflows. Below you’ll find 5 bite‑sized subprojects, each one a mini project demonstrating a unique way to let these agents collaborate on real problems, from plotting stock charts to crafting full reports.

---

## 🛠️ Mini Projects

### 1. Multi-Agent Conversation(Comedy Duo)

**Pattern:** Here, I have taken a Two‑Comedian to chat.

* **Actors:** Cathy & Joe, each a `ConversableAgent` with custom system prompts.
* **Flow:** Joe kicks off with a punchline; Cathy builds on it. They riff back and forth until one says, “I gotta go.”
* **Key features:**

  * `max_turns` control 
  * They exchange jokes, remembering punchlines and building off each other's humor.
  * Termination is dynamic: they stop when one says "I gotta go."
  * Tracks full conversation history, token usage, and allows you to generate summary reflections.
    
---

### 2. Sequential Chats and Customer Onboarding

**Pattern:** Step‑by‑Step Chat Pipeline

* **Use case:** Customer onboarding or ETL pipelines.
* **How it works:** Chain agents in a fixed WelcomeAgent → order—Greeter → DataCollector → Verifier, passing summaries or reflections as context.
* **Benefits:**

  * Modular design: Add or reorder steps by editing a list.
  * Flexible summaries: Quick carryover vs. thoughtful LLM reflections.

---

### 3. Reflection and Blogpost Writing

**Pattern:** Nested Chat Teams

* **Manager agent** spawns a mini‑team on demand.
* **Example:** A news micro‑team with research, drafting, and fact‑checking agents—all coordinated in one chat.
* **Use case:** Collaborative writing, turn‑based games or dynamic task delegation.

---

### 4. ChessMaster(Chess Game between 2 AI Agents)

**Pattern:** Tool-enabled agents with nested chats

* **Agents:** White & Black players using GPT-4 Turbo.
* **Tool:** `BoardProxy` executes `get_legal_moves()` and `make_move()` with python-chess.
* **Flow:** Player asks for moves, proxy returns legal UCI options, player chooses and proxy confirms.

- **Why it's cool:** Combines strategy, tool use, and turn-based coordination inside a conversational loop.

---

### 5. Coding and Financial Analysis

**Pattern:** Code generation + execution loop

* **Roles:** Code Writer drafts Python scripts; Executor runs them locally.
* **Demo task:** Fetch YTD(Year to Date) gains for NVDA/TSLA with `yfinance` and plot via `matplotlib`.

---

### 6. Stock Report Generation

**Pattern:** Group chat with planning and role distribution

* **Team:** Planner → Engineer → Executor → Writer → Admin.
* **Workflow:**

  1. **Planner:** Breaks down tasks: fetch, analyze, draft.
  2. **Engineer:** Writes the python code for each subtask.
  3. **Executor:** Runs that code and returns visuals, stats, etc.
  4. **Writer:** Drafts the final Markdown report
  5. **Admin:** checks progress, requests human approvals.
* **Outcome:**  A complete stock report, with data pulled, charts generated, and blog written—all through agent interaction.

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
