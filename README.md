# Shipping‑Cost Calculator Refactor

## Objective
Refactor the current shipping‑cost calculator so it **meets the full business contract** and **all 15 Jest tests pass** without performance regressions.

---

## What You Must Deliver

### 1. Implementation (`shipping.ts`)
- **Language:** TypeScript  
- **Rename function:** `$$` → `somethingMeaningfulVariableName` (exported from `shipping.ts`)  
- **Rules to satisfy (per existing tests):**
  - Weight‑based charge  
  - Fragile fee  
  - Sunday surcharge  
  - Zero‑qty exclusions  
  - Correct rounding  
  - Input validation with descriptive `Error` messages  
- **Performance:** Handle 1,000,000 line items in **< 200 ms** on standard hardware  
- **Code quality:** No magic numbers, dead code, or artificial slow‑downs  
- **Docs:** Concise JSDoc for parameters, return value, and possible errors

### 2. Tests (`shipping.test.js` / `.ts`)
- Only update the **import path/name** to the new function.  
- **All 15 assertions remain unchanged and must pass.**

### 3. Changelog (`CHANGELOG.md`)
- ≤ 5 lines.  
- Mention the **breaking change** (`$$` ➜ `somethingMeaningfulVariableName`).  
- List bug fixes.  
- Note any anomaly or confusing requirement you encountered.

---

## Deliverables

- `shipping.ts` with the refactored `somethingMeaningfulVariableName` function.  
- Updated `shipping.test.js` (or `.ts`) with the new import path/name (all tests green).  
- `CHANGELOG.md` entry (short, ≤ 5 lines) including anomalies.

---
