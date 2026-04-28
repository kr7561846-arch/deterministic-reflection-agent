Deterministic Reflection Agent

A deterministic, decision-tree-based reflection system that guides users through structured self-analysis across three psychological dimensions:

Locus (Agency) — Victim ↔ Victor
Orientation (Contribution) — Entitlement ↔ Contribution
Radius (Perspective) — Self ↔ Others

This system encodes behavioral psychology into a navigable tree, not an LLM—ensuring predictability, auditability, and consistency.

🚀 Why This Project

Most tools capture what happened.
This system helps users reflect on why it happened and how they showed up.

It is designed as a deterministic reflection engine:

No AI at runtime
No free-text ambiguity
Same inputs → same outputs
🧩 Core Features
✅ Fully deterministic decision tree
✅ Fixed-choice questions (no free text)
✅ Branching logic based on user responses
✅ Signal-based state tracking (axis-wise)
✅ Context-aware reflections using interpolation
✅ Structured end-of-day summary
🏗️ Project Structure
/tree/
  reflection-tree.json      # Tree structure (nodes, transitions, signals)

/agent/
  main.py                   # CLI-based reflection engine

/diagram/
  tree-diagram.png          # Visual representation of the tree

/transcripts/
  persona-1.md              # External / Entitled / Self-centric path
  persona-2.md              # Internal / Contribution / Other-centric path

write-up.md                 # Design rationale
README.md                   # Project documentation
🌳 How It Works

The system operates as a state-driven tree traversal engine:

Node Types
start → session entry
question → user selects from fixed options
decision → routes based on previous answers
reflection → contextual insight
bridge → transitions between axes
summary → final synthesis
end → session close
🔄 Flow of Interaction
Axis 1: Locus (Agency)
   ↓
Axis 2: Contribution (Value)
   ↓
Axis 3: Radius (Perspective)
   ↓
Summary

Each axis:

Surfaces a mindset
Branches based on behavior
Delivers a tailored reflection
🧠 State & Signals

Each response contributes to signals:

axis1: internal / external
axis2: contribution / entitlement
axis3: self / other

These signals:

Influence branching
Shape reflections
Drive the final summary
✨ Example Reflection

"You described reacting to a situation someone else created. That’s real.
But even in that moment — you chose how long to stay there."

🖥️ Running the Agent
1. Install Python (if not already installed)
2. Run the program
python main.py
3. Interact via CLI
Choose options using numbers
Read reflections
Complete the session
📊 Design Philosophy
1. Determinism over Intelligence

No LLMs at runtime.
All intelligence is encoded in structure.

2. Questions Reveal, Not Ask Directly

Instead of:

“Did you take responsibility?”

We use:

“When things slipped today, what did your attention go to first?”

3. Branching Changes Tone, Not Just Flow

Different answers → different psychological interventions

4. Reflection > Judgment

The system:

Does not score
Does not label
Encourages awareness, not guilt
📚 Psychological Foundations
Locus of Control — Julian Rotter
Growth Mindset — Carol Dweck
Psychological Entitlement — W. Keith Campbell
Organizational Citizenship Behavior — Dennis Organ
Self-Transcendence — Abraham Maslow
Perspective-Taking — C. Daniel Batson
🧪 Example Personas
Persona 1:
External locus
Entitlement mindset
Self-focused

→ Reflection highlights awareness of control gaps

Persona 2:
Internal locus
Contribution-driven
Other-oriented

→ Reflection reinforces and expands impact

⚙️ Technical Highlights
JSON-driven architecture
Tree loaded dynamically (not hardcoded)
Regex-based interpolation
Deterministic rule engine
Modular node handling
🔮 Future Improvements
Deeper branching (30–40 nodes)
Multi-day pattern tracking
UI-based interface (web/mobile)
Adaptive summaries based on signal dominance
Visualization of personal growth trends
🧑‍💻 Author

Built as part of a Knowledge Engineering assignment
focused on encoding psychology into deterministic systems.
