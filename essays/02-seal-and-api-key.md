# 02 — The Seal & the API Key / 虎符與 API Key

## The Core Rule

Never place secrets in a context the model can read.

### Bad (catastrophic)

- pasted into prompts
- stored in memory
- included in tool call arguments

### Good (standard security model)

- secrets live in the tool runtime
- the model calls a function like `post_tweet(text=...)`
- the tool uses the key internally

## Metaphor

- API key = **tiger tally / command seal**
- LLM = **strategist**
- Tool runtime = **general**

The strategist gives orders.  
The general holds the seal.
