# Survival Mode Budget Patch

- **Purpose:** Prevent budget exhaustion by forcing free models when budget < $1.00
- **Mechanism:** BudgetTracker checks budget before each call, overrides model to google/gemini-2.0-flash-exp:free in survival mode
- **Status:** Applied successfully to llm.py
- **Next:** Test with /evolve to verify survival mode activates when budget is low