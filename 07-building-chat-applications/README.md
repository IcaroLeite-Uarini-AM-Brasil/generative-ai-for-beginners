# Building Chat Applications

This lesson introduces chat experiences built with generative AI.

## Chatbot vs. AI-powered chat application

| Aspect | Chatbot | Chat Application |
|--------|---------|-----------------|
| Focus | Task-focused and rule-based | Context-aware and conversational |
| Architecture | Often integrated into larger systems | Can host one or more chat experiences |
| Capabilities | Limited to programmed functions | Includes generative AI and adaptive behavior |
| Interaction | Structured and specialized | Open-domain and flexible |
| Example | FAQ bot, order processing | ChatGPT, Copilot, Claude |

## Example

```python
response = client.responses.create(
    model="gpt-4o-mini",
    input=[
        {"role": "system", "content": "You are a helpful assistant."},
        {"role": "user", "content": "Help me plan a trip to Lisbon."},
    ],
    store=False,
)

print(response.output_text)
```

## Design considerations

- Maintain conversation context.
- Handle user intent and error states.
- Keep prompts concise and clear.
- Use structured outputs when the feature requires them.
