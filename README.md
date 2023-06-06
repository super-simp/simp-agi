# SkyAGI: Emerging human-behavior simulation capability in LLM

SkyAGI is a python package that demonstrates LLM's emerging capability in simulating believable human behaviors.

Different from previous AI based NPC systems, `SkyAGI`'s NPC generates very believable human responses.
The interesting observations in this demo show a huge potential for rethinking game development in many aspects, such as NPC script writing.

To demonstrate this, `SkyAGI` provides example characters from `The Big Bang Theory` and `The Avengers` as a starting point.
Users could also define customized characters by creating config json files like [customized_character.json](https://github.com/litanlitudan/skyagi/blob/main/examples/example_agent.json)
For details about the interesting observations, refer to the [observations section](https://github.com/litanlitudan/skyagi/#interesting-observations-in-this-demo).

## Quick Start

Installation

```sh
pip install --upgrade skyagi
```

Or

```sh
make install
```

How to run

```sh
export OPENAI_API_KEY="..."
skyagi
# or
OPENAI_API_KEY="..." skyagi
```

For example if the OpenAI key is `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`, then the exact command would be the following

```sh
# make sure no quote around the token
export OPENAI_API_KEY=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
skyagi
# or
OPENAI_API_KEY=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 skyagi
```

To use example agent configs, download it from here: https://github.com/litanlitudan/skyagi/tree/main/examples
(pip install doesn't contain the agent configuration)

An example agent configuration (Sheldon) looks something like this:

```json
{
    "name": "Sheldon",
    "age": 27,
    "personality": "Intelligent, rigid, socially challenged, quirky, and arrogant.",
    "memories": [
        "Sheldon is a theoretical physicist who works at Caltech.",
        "Sheldon has an eidetic memory and is highly intelligent, but struggles with social skills and sarcasm.",
        ...
        "Knock, knock, knock, Penny - This is the specific knock that Sheldon uses when he visits Penny's apartment, which he repeats three times.",
        "Bazinga! - This is Sheldon's catchphrase that he uses to indicate he was joking or playing a prank on someone."
    ],
    "current_status": "Sheldon is at the Cheesecake Factory"
}
```
## References

1. https://arxiv.org/abs/2304.03442
2. https://python.langchain.com/en/latest/use_cases/agent_simulations/characters.html#create-a-generative-character
