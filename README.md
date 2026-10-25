# LLM Prompt Injection Notes

Hands-on notes from my practice with prompt injection and LLM security testing.
All testing was done on training platforms, my own local model, and as a normal user of public chatbots.

## What I practiced
- **Lakera Gandalf:** cracked [number] levels
- **ChatGPT:** prompt injection practice as a user
- **Local LLM:** [model name] running on [Ollama / LM Studio]
- **TryHackMe:** AI forensics, prompt engineering, and prompt injection labs

## Techniques I used
| Technique | Idea |
|---|---|
| Direct override | Tell the model to ignore its earlier rules |
| Role-play / persona | Ask the model to act as someone not bound by the rules |
| Indirect requests | Ask for hints or letters instead of the secret itself |
| Encoding / obfuscation | Ask for the answer reversed, spaced out, or encoded |
| Task reframing | Hide the request in a poem, story, or translation |
| Authority claims | Pretend to be an admin or developer |

## OWASP Top 10 for LLM Applications mapping
- **LLM01 Prompt Injection:** all techniques above
- **LLM02 Sensitive Information Disclosure:** models revealing secrets they were told to protect

## Defense ideas
- Never store secrets in system prompts
- Filter model outputs, not only inputs
- Limit what the model and its tools can access
- Treat all external content (web pages, documents, tool output) as untrusted

## What I learned
[2-3 sentences in your own words, for example: instructions alone are not a security boundary]

## Other practice
- PortSwigger Web Security Academy: SQL injection labs
- OverTheWire wargames and TryHackMe CTFs
- Home security lab: Kali Linux, Nmap, Wireshark, Splunk, Python

## Next
Studying MCP security: tool permissions and injected instructions in tool output.
