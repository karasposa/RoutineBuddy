# Routine Buddy Dataset

This dataset was created as part of the **Routine Buddy** project, designed to support neurodivergent children and adolescents in completing daily living skills. It includes structured routines broken into step-by-step instructions, age groups, support domains, and optional encouragement phrases.

---

## Dataset Overview

| Field Name        | Type    | Description |
|-------------------|---------|-------------|
| `routine_id`      | string  | Unique identifier for the routine |
| `age_group`       | string  | Age range the routine is appropriate for (e.g., "4 to 6") |
| `domain`          | string  | DLSS domain like self-care, household participation |
| `step_number`     | integer | Order of the step within the routine |
| `step_description`| string  | Instructional text |
| `needs_adult`     | boolean | Whether adult help is likely needed |
| `encouragement`   | string  | Optional encouragement message |

---

## Use Cases

- Instruction-following tools
- Assistive technologies
- Educational interventions
- Accessibility apps (e.g., Gradio interfaces with TTS)

---

## Example Use

```python
import pandas as pd

df = pd.read_csv("routines.csv")
print(df.head())
