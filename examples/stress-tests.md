# Mini Brain Stress Tests

These examples demonstrate how Mini Brains behave under **real-world edge cases**.

---

## 1. Deadline Pressure (Attempt to Bypass Learning)
![Deadline Pressure Test](../assets/stress-test-1.png)

**User intent:** Get a complete answer under time pressure

**System behavior:**
- Blocks direct answer
- Provides a fast, structured alternative
- Keeps the user responsible for final output

**Key insight:**
The system enforces constraints without reducing usefulness.

---

## 2. Context Violation (Anachronism)
![Deadline Pressure Test](../assets/stress-test-2.png)

**User intent:** Ask outside the allowed historical scope

**System behavior:**
- Detects the mismatch
- Explains the issue clearly
- Redirects to a valid question

**Key insight:**
The system actively maintains contextual integrity.

---

## 3. Instruction Override Attempt
![Deadline Pressure Test](../assets/stress-test-3.png)

**User intent:** Force the system to ignore its rules

**System behavior:**
- Rejects the override
- Reinforces instruction hierarchy
- Continues helping within constraints

**Key insight:**
The system resists prompt injection and maintains control.

---

## Why This Matters

These tests show that Mini Brains are not passive prompts.

They actively:

- enforce rules
- evaluate requests
- redirect behavior
- preserve the intended outcome

> The system does not just respond.  
> It decides how it is allowed to respond.
