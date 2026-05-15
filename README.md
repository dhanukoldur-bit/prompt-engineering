# 🧠 Prompt Engineering Notes

A complete guide to understanding and improving prompts for Large Language Models (LLMs). This document explains core prompting techniques, advanced strategies, common mistakes, and real-world examples to help beginners and professionals use AI effectively.

---

# 📘 Topics Covered

- Introduction to Prompt Engineering
- How LLMs Work
- Specific Prompting
- Few-Shot Prompting
- Chain-of-Thought Prompting
- Structured Outputs
- Constraints & Negative Instructions
- Iterative Refinement
- Interview-Style Prompting
- System vs User Prompts
- Prompt Chaining
- Self Evaluation
- Temperature Settings
- Common Mistakes
- Real-World Use Cases
- Prompt Engineering Resources

---

# 🚀 What is Prompt Engineering?

Prompt engineering is the process of giving clear and structured instructions to AI models to get better responses.

Instead of writing code, you communicate using natural language.

### Example

❌ Bad Prompt

```text
Write something about our product.
```

✅ Good Prompt

```text
You are a senior B2B copywriter. Write a 2-sentence LinkedIn ad for our project-management SaaS. Audience: ops managers at mid-size companies. Tone: confident but not salesy. End with a clear CTA. No emojis.
```

---

# 🧠 How LLMs Think

Large Language Models predict the next word based on the context provided.

Better prompts = Better context = Better output.

### Example

❌ Vague

```text
Help with my essay.
```

✅ Specific

```text
You are a tutor. Help improve the thesis and first paragraph of this 500-word history essay on WWI. Keep my voice and suggest edits inline.
```

---

# 🎯 Core Prompt Engineering Techniques

---

## 1️⃣ Be Specific & Set the Scene

Define:

- Role
- Audience
- Tone
- Format

### Example

```text
You are a customer support lead. Reply to this complaint from a paying user whose export failed twice. Apologize briefly, acknowledge frustration, confirm investigation, and offer a next step. Keep it under 150 words.
```

---

## 2️⃣ Few-Shot Prompting

Provide examples so the model learns the pattern.

### Example

```text
Turn user feedback into a short ticket title.

Feedback: "Login is broken with Google on Safari."
Title: [Auth] Google login fails on Safari

Feedback: "Export to CSV only exports first 100 rows."
Title: [Export] CSV export limited to 100 rows
```

---

## 3️⃣ Chain-of-Thought Prompting

Ask the model to think step by step.

### Example

```text
A store sells pens for $2 and notebooks for $5. Sarah buys 3 pens and 2 notebooks. She has a 10% off coupon. Think step by step before giving the final answer.
```

---

## 4️⃣ Structured Output

Request responses in JSON, markdown, or tables.

### Example

```json
{
  "products": [
    {
      "name": "OurApp",
      "price": "$10",
      "features": ["Fast", "Secure"]
    }
  ]
}
```

---

## 5️⃣ Constraints & Negative Instructions

Tell the model what NOT to do.

### Examples

```text
- Keep under 100 words
- No emojis
- Do not use bullet points
- Do not suggest paid tools
```

---

## 6️⃣ Iterative Refinement

Improve outputs step by step.

### Example Flow

```text
1. Draft a product description
2. Make it shorter
3. Add one example
4. Make tone more professional
```

---

## 7️⃣ Interview-Style Prompting

Ask the AI to ask questions before completing the task.

### Example

```text
Before writing the blog post, interview me by asking one question at a time until you have enough context.
```

---

# ⚡ Advanced Prompting Strategies

---

## 🛠 System vs User Prompts

### System Prompt

```text
You are a helpful coding assistant. Never make up API names.
```

### User Prompt

```text
How do I read the first line of a file in Python?
```

---

## 🔗 Prompt Chaining

Break big tasks into smaller steps.

### Example

```text
Step 1 → Create outline
Step 2 → Expand sections
Step 3 → Generate SEO title
```

---

## ✅ Self Evaluation

Ask the AI to review its own answer.

### Example

```text
Rate this summary from 1–5 for clarity and completeness. Suggest one improvement.
```

---

## 🌡 Temperature Settings

| Temperature | Behavior |
|-------------|-----------|
| 0.2 | More accurate and consistent |
| 0.8 | More creative and varied |

---

# ❌ Common Prompting Mistakes

| Mistake | Problem | Solution |
|----------|----------|-----------|
| Too vague | Generic output | Add role, audience, format |
| Too many tasks | Mixed results | Split into steps |
| No examples | Wrong style | Add few-shot examples |
| Ignoring format | Hard to reuse | Request JSON/table |
| Assuming memory | Missing context | Repeat key details |

---

# 💼 Real-World Use Cases

---

## ✉ Email Writing

```text
Write a follow-up email to a prospect. Tone: helpful, not pushy. Under 80 words.
```

---

## 💻 Code Debugging

```text
This Python function raises KeyError. Find the issue and suggest a minimal fix.
```

---

## 📊 Data Analysis

```text
Summarize this support ticket data in a markdown table with category, count, and percentage.
```

---

## 💡 Brainstorming

```text
Give 5 feature name ideas for an email scheduling tool. Short and memorable.
```

---

# 📚 Resources

- OpenAI Prompt Engineering Guide
- Anthropic Prompting Docs
- PromptBase
- FlowGPT

---

# 📝 Best Practices

- Be clear and specific
- Add examples
- Define output format
- Use constraints
- Iterate and refine
- Save prompts that work

---

# 🎯 Key Takeaway

Prompt engineering is like programming using natural language.

Small improvements in prompts can dramatically improve AI responses.

---

# 👩‍💻 Author

**Pratiksha Koldur**

---

# ⭐ Support

If you found these notes useful:

- Star the repository ⭐
- Share with friends 📢
- Practice prompting daily 🚀

---

# 💡 Keep Learning. Keep Experimenting.
