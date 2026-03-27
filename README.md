# ReAct Agent
A simple ReAct (Reason + Act) agent built from scratch using OpenAI.

## What it does
* Takes user input
* Uses LLM to reason
* Decides actions (tools)
* Executes tools
* Uses observations to give final answer

---

## Functions (Tools)

### 1. get_capital_city

* Input: country name
* Output: capital city

Example:

```text
get_capital_city: Lithuania → Vilnius
get_capital_city: Japan → Tokyo
```

---

### 2. get_popular_places

* Input: city name
* Output: popular tourist places

Example:

```text
get_popular_places: London → Big Ben, London Eye
```

---

### 3. get_other_cities_in_the_country

* Input: country name
* Output: list of other cities

Example:

```text
get_other_cities_in_the_country: United Kingdom → Manchester, Birmingham
```

---

## How to run

```bash
pip install openai
python react_agent.py
```

---

## Example

```text
User: I want to visit Lithuania

Agent:
Action: get_capital_city: Lithuania  
Observation: Vilnius  

Action: get_popular_places: Vilnius  
Observation: Gediminas Tower, Old Town  

Final Answer: You can visit Vilnius and explore Gediminas Tower and Old Town.
```

---

## Files

* `react_agent.py` → main code
* `README.md` → documentation
=======
# react_agent
>>>>>>> 87b7967e15590e819bb074cccef2a58ae83645b5
