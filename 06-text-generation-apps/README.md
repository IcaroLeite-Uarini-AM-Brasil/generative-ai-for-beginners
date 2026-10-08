# Building Text Generation Applications

This lesson shows how to build applications that generate text using language models.

## Using the correct model

The code samples should use a valid model name:

```python
response = client.responses.create(
    model="gpt-4o-mini",
    input=prompt,
    store=False,
)
```

## Example app

```python
from openai import OpenAI

client = OpenAI()
prompt = "Write a short product announcement for a new AI assistant"

response = client.responses.create(
    model="gpt-4o-mini",
    input=prompt,
    store=False,
)

print(response.output_text)
```

## Common patterns

- Generate summaries
- Draft emails
- Create marketing copy
- Expand prompts into structured output

## Troubleshooting

- Verify the API key is configured correctly.
- Check that the deployment name matches the target model.
- Use a known supported model such as `gpt-4o-mini`.
