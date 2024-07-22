# Prompts for CSCW submission #3843.

This repository contains the prompts described throughout the paper titled: "Collecting Qualitative Data at Scale with Large Language Models: A Case Study." Following is a description of each file.

- `member_checker.prompt`: Utilized in the Member Checker condition to summarize the conversation and member check (described in Section 3).
- `participant_persona.prompt`: Utilized in the iterative development of prompts to simulate conversations between the prober and an artificial participant (described in Section 3).
- `dynamic_prober.prompt`: Utilized to create follow-ups dynamically (described in Section 3).
- `qual_coding.prompt`: Utilized to evaluate the LLM's ability to qualitatively code segments (described in Section 5.4).
    - `zero-shot` includes no coded examples.
    - `one-shot` includes 4 coded examples.
    - `few-shot` includes 8 coded examples.
 
## {{$variable}} Notation

The prompting was done using the [Semantic Kernel](https://learn.microsoft.com/en-us/semantic-kernel/overview/) package. To include variables in a prompt, Semantic Kernel employs the {{$}} notation. For example, {{$chat_segment}} would dynamically include the value of the `chat_segment` variable at runtime.
