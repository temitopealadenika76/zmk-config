# GitHub Copilot Planning Prompt Template

Copy everything below the line, replace the placeholder with your task, and paste into Copilot Chat.

---

I need you to create a detailed, implementation-ready plan before taking any action. Format your response as a structured markdown document following this outline. Do not start coding until I approve the plan.

## My Task

[Describe your task or goal here. Include as much context as you have: what's broken, what you want to achieve, any constraints, relevant file paths, or prior attempts.]

---

## Required Plan Structure

Produce a plan document that includes all of the following sections:

### 1. Frontmatter (if supported)

```yaml
---
name: [Short plan name]
overview: [1-2 sentence summary of the goal]
todos: []
---
```

### 2. Problem Statement / Current State

- What exists today? What is broken or inadequate?
- List specific pain points with concrete examples (file paths, line numbers, error messages, workarounds)
- Include any relevant protocol/spec/hardware details in tables if applicable

### 3. Target State

- What should the system look like when done?
- List success criteria clearly

### 4. Current vs. Proposed Comparison

For each major area of change, use a "Now vs. After" format:

**Now:** Current behavior, limitations, workarounds
**After:** New behavior, concrete improvements, what gets eliminated

### 5. Architecture (if relevant)

Include a Mermaid diagram showing:
- Current flow/architecture
- Proposed flow/architecture
- How they differ

### 6. Implementation Plan

Break into numbered phases or steps. For each step:

- **What:** Clear description of the work
- **Files:** Specific file paths to modify
- **Code snippets:** Actual YAML/JavaScript/Python/etc. for proposed changes where helpful
- **Dependencies:** What must be done first
- **Verification:** How to confirm the step is complete

### 7. Key Files Summary Table

| File | Changes |
|------|---------|
| `path/to/file1` | Brief description of edits |
| `path/to/file2` | Brief description of edits |

### 8. Edge Cases & Risks

- Potential failure modes
- Backward compatibility considerations
- Graceful degradation if something fails
- What to do if X doesn't work

### 9. Optional / Future Work

Items explicitly out of scope for this plan but worth noting for later.

### 10. Validation

- How to verify the full solution works
- Tests to run or add
- Manual checks to perform

---

Respond with the complete plan document. Wait for my approval before implementing.
