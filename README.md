## Quick Start

pip install --upgrade skyagi

Or
make install

# RUN

export OPENAI_API_KEY="..."
skyagi

# or

OPENAI_API_KEY="..." skyagi

Example: if the OpenAI key is `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`, then the exact command would be the following

# make sure no quote around the token

export OPENAI_API_KEY=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
skyagi

# or

OPENAI_API_KEY=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 skyagi

# EXAMPLE AGENT CONFIGURATION

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
