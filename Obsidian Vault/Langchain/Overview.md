characteristics of Lang chain
- streaming
- human in the loop - confirmation by the human
- generative UI components

Demo
- lang graph cloud - platform for deploying Lang graph agents and assistant UI
	- what is the revenue of apple - streamin
	- stock of the apple - generative UI component
	- buy me a five stocks - human in the loop
assitant - ui
- react component library for chatbot like UI's

**Lang graph studio to what looks like visually**

![[Pasted image 20240916113913.png]]
# Add observability to your LLM application

## Observability for LLM Applications

### Key Points

- **Importance of Observability:**
    - Essential for LLM applications due to their non-deterministic nature.
    - Helps in debugging unexpected results and ensuring application reliability.
- **LangSmith's Role:**
    - Provides LLM-native observability tools.
    - Offers meaningful insights into LLM application behavior.
- **Observability Throughout Application Development:**
    - Critical at all stages: prototyping, beta testing, and production.
    - Considerations vary at each stage but are interconnected.

### Summary

LangSmith's LLM-native observability is crucial for debugging and understanding the behavior of LLM applications. This is especially important due to the non-deterministic nature of LLMs. Observability is essential throughout the application development lifecycle, from early prototyping to production.


# setting up observability
## Prototyping
- Set up your environment
	- install the LangSmith SDK
	- set up the appropriate environment variables
	- Trace your LLM calls
		- Notice how we import `from langsmith.wrappers import wrap_openai` and use it to wrap the OpenAI client (`openai_client = wrap_openai(OpenAI())`).
	- Trace the retrieval step
		- There's one last part of the application we haven't traced - the retrieval step! Retrieval is a key part of LLM applications
## 