# RAG and Vector Databases

This lesson explains retrieval augmented generation and vector search.

## Re-ranking logic

The retrieval example should iterate over valid document indices without reusing the loop variable incorrectly.

```python
# Find the most similar documents
distances, indices = nbrs.kneighbors([query_vector])

# Print the most similar documents
for i in range(min(3, len(indices[0]))):
    index = indices[0][i]
    try:
        print(f"Document {i + 1}:")
        print(f"  Chunk: {flattened_df['chunks'].iloc[index]}")
        print(f"  Path: {flattened_df['path'].iloc[index]}")
        print(f"  Distance: {flattened_df['distances'].iloc[index]}\n")
    except IndexError:
        print(f"Index {index} not found in DataFrame")
```

## Valid model example

```python
response = client.responses.create(
    model="gpt-4o-mini",
    input="Summarize the top retrieved chunks for this query.",
    store=False,
)
```

## Key concepts

- Chunking documents into manageable pieces
- Embedding text into vector space
- Finding semantic matches with nearest neighbors
- Combining retrieval with generation

## Best practices

- Keep chunk size consistent.
- Store metadata for filtering and traceability.
- Validate index ranges before accessing rows.
- Prefer explicit error handling around retrieval results.
