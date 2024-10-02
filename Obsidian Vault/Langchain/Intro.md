Langchain

- prompt template
- chain - important object 
- sequential chain - restaurant name as input, it will give menu items
![[Pasted image 20240917142852.png]]

input of 2 step is output of 1 step

## components
- schema
	- systemmessage
	- humanmessage
- Documents
	- An object that holds a piece of text and metadata (more information about that text)
	- schema.component
- Models
	- language model
		- OpenAI
	- Chat model
		- ChatOpenAI
	- Function calling methods
		- Function calling models are similar to Chat Models but with a little extra flavor. They are fine tuned to give structured data outputs.
	- Text embedding model
		- Change your text into a vector (a series of numbers that hold the semantic 'meaning' of your text). Mainly used when comparing two pieces of text together.
- Prompts
	- Text generally used as instructions to your model
	- Prompt Template
		- An object that helps create prompts based on a combination of user input, other non-static information and a fixed template string.
		- 

## use cases
- chatbots
- summarizations
- question answerings
- data augmentation - generate synthetic data
- virtual agents

## conceptual

- ## LangChain Architecture Overview

### Core Packages

- **langchain-core:** Defines fundamental abstractions for components like LLMs, vector stores, and retrievers.
- **langchain:** Focuses on chains, agents, and retrieval strategies that form the cognitive architecture of an application.
- **langchain-community:** Contains third-party integrations maintained by the community, including various components like LLMs, vector stores, and retrievers.

### Partner Packages

- **langchain-openai**, **langchain-anthropic**, etc.: Provide specialized support for popular integrations.

### Extensions

- **langgraph:** Enables building robust and stateful multi-actor applications with LLMs using a graph-based approach.
- **langserve:** Facilitates deploying LangChain chains as REST APIs for production use.

## Langsmith

- developer platform that lets youdebug, text, evaluate and monitor llm application
![[Pasted image 20240920161714.png]]

# LCEL - `LangChain Expression Language`

- **First-class streaming support**
	- chains with LCEL you get the best possible time-to-first-token
	- stream tokens straight from an LLM to a streaming output parser
- **Async support**
	- 