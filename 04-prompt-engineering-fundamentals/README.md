# Prompt Engineering Fundamentals

This lesson demonstrates the core principles for writing effective prompts.

## Model configuration

Use the supported Azure OpenAI model for the examples below:

```python
response = client.responses.create(
    model="gpt-4o-mini",
    input=prompt,
    store=False,
)
```

## Why this matters

Prompt engineering is the process of designing inputs so a model follows instructions, stays within constraints, and returns the expected format.

## Best practices

- Be specific about the task and output format.
- Include context, constraints, and examples when useful.
- Ask for structured output when the task needs it.
- Iterate with short, observable prompt changes.

## Example

```python
prompt = """
You are a customer support assistant.
Answer in 3 bullet points.
Keep the tone professional and concise.
Avoid technical jargon.
"""
```

## Notes

This curriculum standardizes on `gpt-4o-mini` for the examples in this lesson to avoid invalid model references.
