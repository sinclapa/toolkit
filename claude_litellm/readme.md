# Claude and LiteLLM

## Setup
```bash
pip install 'litellm[proxy]'
```

## Runn
```bash
litellm --config copilot-config.yaml
```

## Test

```bash
curl --location 'http://localhost:4000/chat/completions' --header 'Content-Type: application/json' --header 'Editor-Version: CommandLine/1.0' --data '{
  "model": "claude-haiku",
  "messages": [
    {
      "role": "user",
      "content": "what llm are you"
    }
  ]
}
```

## References
https://code.claude.com/docs/en/overview
https://blog.f12.no/wp/2025/09/22/using-claude-code-with-github-copilot-a-guide/