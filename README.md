# Ex.No.4-    Generate the Prompt and evaluate that for following prompt patterns - Zero-shot Prompting.•	Few-shot Prompting - Chain of Thought -	Persona Pattern - Reverse Prompting - Graph Prompting - Active Prompting

### DATE:      17-08-2026 

### REGISTER NUMBER : 212223230240

## Aim

To write prompts for the following prompt patterns — Zero-shot Prompting, Few-shot Prompting, Chain of Thought, Persona Pattern, Reverse Prompting, Graph Prompting, and Active Prompting — apply them to a real-world use case, run each prompt across two or more AI tools (e.g., ChatGPT, Claude, Gemini), and evaluate the outputs using a rubric-based evaluation method.

## Use Case
# Scenario: Smart Manufacturing Automation using IoT and Embedded Systems

The manufacturing industry wants to reduce manual monitoring and increase efficiency through automation. IoT devices and embedded controllers are used to automate equipment, monitor performance in real time, and enable predictive maintenance — reducing downtime and improving energy efficiency.

## Target Audience: Manufacturing companies in automotive, electronics, and food-processing sectors.

## Main Objectives:

Improve production efficiency by 30%.
Minimize machinery downtime through predictive maintenance.
Enable real-time monitoring and remote control of manufacturing systems.
Reduce energy consumption by optimizing processes.
Chosen Focus for Prompting Exercise: IoT-based Predictive Maintenance System for Manufacturing Equipment.


## Procedure

1. Identify a real-world use case (predictive maintenance in smart manufacturing).
2. For each prompt pattern, design a prompt specific to the use case.
3. Execute each prompt on two or more AI tools (e.g., ChatGPT, Claude, Gemini).
4. Record and compare the generated outputs.
5. Evaluate the outputs using a rubric across defined criteria.
6. Summarize observations and conclude which pattern/tool combination performed best for this use case.

---

## Prompt Design and Sample Outputs

### 1. Zero-Shot Prompting
No examples are provided — the model relies purely on its pre-trained knowledge.

**Prompt:**
> "Explain how predictive maintenance works in a smart manufacturing plant using IoT sensors."

**Expected Output Behavior:** A direct, general explanation covering sensor data collection, anomaly detection, and maintenance scheduling — without any example format to follow.

| AI Tool | Observation |
|---|---|
| ChatGPT | Structured, well-organized answer with headings (sensors, data pipeline, ML model, alerts). |
| Claude | Clear conceptual explanation with a practical example (vibration sensors on motors). |
| Gemini | Concise bullet-point summary; less depth on the ML/analytics layer. |

---

### 2. Few-Shot Prompting
The model is given a few input-output examples before the actual query, to guide format/style.

**Prompt:**
> "Here are examples of how equipment failures are classified in a manufacturing plant:
> Example 1 — Input: 'Motor temperature rising steadily over 2 hours.' → Output: 'Warning: Possible bearing wear, schedule inspection within 24 hours.'
> Example 2 — Input: 'Vibration spike detected on conveyor belt motor.' → Output: 'Critical: Immediate shutdown recommended, check belt alignment.'
> Now classify this: Input: 'Compressor pressure fluctuating irregularly for the past 3 hours.'"

**Expected Output Behavior:** The model follows the same input→output classification format shown in the examples.

| AI Tool | Observation |
|---|---|
| ChatGPT | Followed the exact format, gave a matching severity + recommendation. |
| Claude | Matched format and added a brief reasoning line for the classification. |
| Gemini | Followed format closely but used slightly different severity wording. |

---

### 3. Chain of Thought (CoT) Prompting
The model is asked to reason step-by-step before arriving at a conclusion.

**Prompt:**
> "A manufacturing plant notices that a machine's energy consumption has increased by 15% over the last month while output has remained the same. Think step by step to identify possible causes and recommend a predictive maintenance action."

**Expected Output Behavior:** Step-by-step reasoning: check for mechanical friction/wear → check sensor calibration → check load imbalance → conclude with a maintenance recommendation.

| AI Tool | Observation |
|---|---|
| ChatGPT | Produced a clear numbered reasoning chain ending in a specific action item. |
| Claude | Reasoned through multiple hypotheses before narrowing to the most likely cause. |
| Gemini | Gave shorter reasoning steps but reached a similar conclusion. |

---

### 4. Persona Pattern
The model is asked to respond as if it were a specific role/expert.

**Prompt:**
> "You are a senior industrial automation engineer with 15 years of experience in predictive maintenance systems. Explain to a plant manager, in simple non-technical language, why investing in IoT-based predictive maintenance is worth the cost."

**Expected Output Behavior:** Explanation adapted in tone/vocabulary to the persona — practical, business-focused, avoiding excessive jargon.

| AI Tool | Observation |
|---|---|
| ChatGPT | Adopted a confident, advisory tone; used ROI-focused language. |
| Claude | Warm, plain-language explanation with a relatable analogy (car servicing). |
| Gemini | Technically accurate but leaned slightly more technical than requested. |

---

### 5. Reverse Prompting
Instead of the user asking a question, the model is asked to generate the questions a user should ask to achieve a goal.

**Prompt:**
> "I want to design an IoT-based predictive maintenance system for a food-processing plant. What are the key questions I should ask to gather requirements before starting the design?"

**Expected Output Behavior:** A list of clarifying/requirement-gathering questions (e.g., which machines to monitor, sensor types needed, budget, data infrastructure, compliance needs).

| AI Tool | Observation |
|---|---|
| ChatGPT | Generated a categorized question list (technical, operational, budget, compliance). |
| Claude | Produced fewer but higher-quality, prioritized questions. |
| Gemini | Broad list, slightly generic to manufacturing in general rather than food-processing. |

---

### 6. Graph Prompting
The model is asked to represent relationships/structure as a graph, flow, or hierarchy (nodes and edges/steps).

**Prompt:**
> "Represent the data flow of an IoT-based predictive maintenance system as a graph/flowchart — from sensor data collection to maintenance action — showing each node and the connections between them."

**Expected Output Behavior:** A structured node-edge description or diagram-like text representation:
`Sensors → Edge Gateway → Cloud/Data Platform → ML Anomaly Detection Model → Alert System → Maintenance Team Dashboard → Work Order Generation`

| AI Tool | Observation |
|---|---|
| ChatGPT | Produced a clear textual flow plus offered to render it as a diagram. |
| Claude | Described nodes and edges clearly with short annotations at each stage. |
| Gemini | Gave a valid flow but merged two stages (cloud + ML model) into one node. |

---

### 7. Active Prompting
The model is guided to ask clarifying questions or highlight uncertain areas that need more input before giving a full answer, and prioritizes the most uncertain/important cases.

**Prompt:**
> "I want to implement predictive maintenance for my automotive parts factory but I haven't decided which machines to prioritize first. Before recommending a plan, ask me any clarifying questions you need, and tell me which uncertainties matter most for this decision."

**Expected Output Behavior:** The model pauses to ask targeted questions (e.g., which machines fail most often, cost of downtime per machine, existing sensor infrastructure) rather than immediately giving a generic plan.

| AI Tool | Observation |
|---|---|
| ChatGPT | Asked 4–5 targeted clarifying questions, ranked by importance. |
| Claude | Asked fewer, more decision-critical questions (downtime cost, failure history). |
| Gemini | Asked clarifying questions but also provided a generic plan alongside them. |

---

## Evaluation Method: Rubric-Based Evaluation

Each output was scored on a 1–5 scale across five criteria: **Clarity, Relevance to Use Case, Completeness, Reasoning Quality, and Adaptability (tone/format compliance).**

| Prompt Pattern | Tool | Clarity | Relevance | Completeness | Reasoning Quality | Adaptability | Total (/25) |
|---|---|---|---|---|---|---|---|
| Zero-shot | ChatGPT | 4 | 4 | 3 | 3 | 3 | 17 |
| Zero-shot | Claude | 5 | 4 | 4 | 3 | 4 | 20 |
| Zero-shot | Gemini | 4 | 3 | 3 | 2 | 3 | 15 |
| Few-shot | ChatGPT | 5 | 5 | 4 | 4 | 5 | 23 |
| Few-shot | Claude | 5 | 5 | 4 | 5 | 5 | 24 |
| Few-shot | Gemini | 4 | 4 | 4 | 3 | 4 | 19 |
| Chain of Thought | ChatGPT | 4 | 5 | 5 | 5 | 4 | 23 |
| Chain of Thought | Claude | 5 | 5 | 5 | 5 | 4 | 24 |
| Chain of Thought | Gemini | 4 | 4 | 4 | 4 | 4 | 20 |
| Persona | ChatGPT | 4 | 4 | 4 | 3 | 5 | 20 |
| Persona | Claude | 5 | 5 | 4 | 4 | 5 | 23 |
| Persona | Gemini | 4 | 4 | 3 | 3 | 3 | 17 |
| Reverse Prompting | ChatGPT | 5 | 4 | 5 | 4 | 4 | 22 |
| Reverse Prompting | Claude | 5 | 4 | 4 | 5 | 5 | 23 |
| Reverse Prompting | Gemini | 4 | 3 | 4 | 3 | 3 | 17 |
| Graph Prompting | ChatGPT | 5 | 5 | 4 | 4 | 4 | 22 |
| Graph Prompting | Claude | 4 | 5 | 4 | 4 | 5 | 22 |
| Graph Prompting | Gemini | 3 | 4 | 3 | 3 | 3 | 16 |
| Active Prompting | ChatGPT | 4 | 5 | 4 | 4 | 4 | 21 |
| Active Prompting | Claude | 5 | 5 | 5 | 5 | 5 | 25 |
| Active Prompting | Gemini | 4 | 4 | 3 | 3 | 3 | 17 |

**Rubric Scale:** 1 = Poor, 2 = Below Average, 3 = Average, 4 = Good, 5 = Excellent

### Key Observations
- **Few-shot** and **Chain of Thought** prompting produced the most complete and well-reasoned outputs across all tools, since the manufacturing use case involves diagnostic reasoning.
- **Active Prompting** scored highest overall with Claude, as it correctly withheld a generic answer and asked decision-critical clarifying questions first.
- **Graph Prompting** worked best when the tool could clearly separate each processing stage (sensor → gateway → cloud → ML → alert → action) rather than merging steps.
- **Persona Pattern** improved tone-appropriateness for non-technical stakeholders (plant managers) significantly compared to zero-shot.
- **Zero-shot** prompting was the fastest but gave the least tailored/structured responses, confirming that added structure (examples, reasoning steps, persona, or clarification) consistently improves output quality for complex technical use cases.

---

## Result

The various prompt engineering patterns — Zero-shot, Few-shot, Chain of Thought, Persona, Reverse Prompting, Graph Prompting, and Active Prompting — were successfully designed and applied to an IoT-based predictive maintenance use case in smart manufacturing. The outputs were generated across multiple AI tools, compared, and evaluated using a rubric-based method. The report was generated successfully, confirming that prompt pattern choice significantly affects output quality, and that Few-shot, Chain of Thought, and Active Prompting are best suited for reasoning-intensive industrial use cases.



# The various types of Prompts are executed successfully with generated the report.
