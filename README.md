# dbt-fusion_learn

Practice project for exploring the **dbt Fusion Engine** locally with **dbt Core**.

This repository contains a simple dbt project designed to help me learn how to run,
test, and deploy dbt models using Fusion’s new execution engine while keeping a
workflow similar to the official *dbt Cloud Developer Path* tutorial.

---

## 🎯 Objectives

- Understand how the **dbt Fusion Engine** differs from the classic dbt runner.
- Build and run models on **Snowflake** using dbt Core from VS Code.
- Practice common developer tasks:  
  - Sources, staging and marts layers  
  - Tests, documentation, and exposures  
  - Incremental models and Jinja macros

---

## 🗂 Project Structure

```bash
dbt_fusion_learn/
│
├─ models/ # Staging + marts layers
│ ├─ staging/
│ └─ marts/
│
├─ macros/ # Custom Jinja macros
├─ seeds/ # Optional seed CSVs
├─ snapshots/ # (if used)
└─ tests/ # Generic & singular tests
```


---

## ⚡️ Requirements

* **dbt-core >= 1.8** (Fusion is enabled by default in recent versions)
* **dbt-snowflake adapter**
* Python 3.9+  
* A Snowflake account with a database and warehouse you can use.

---

## 🔧 Local Setup

Clone this repo and install dependencies:

```bash
git clone https://github.com/danielryvero/dbt-fusion_learn.git
cd dbt-fusion_learn
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt  # or pip install dbt-snowflake
