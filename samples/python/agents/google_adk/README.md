## Google ADK Agent

This sample uses the Google Agent Development Kit (ADK) to create a simple "Expense Reimbursement" agent that is hosted as an A2A server.

This agent takes text requests from the client and, if any details are missing, returns a webform for the client (or its user) to fill out. After the client fills out the form, the agent will complete the task.

## Prerequisites

- Python 3.9 or higher
- UV
- Access to an LLM and API Key


## Running the Sample

1. Navigate to the samples directory:
    ```bash
    cd samples/python
    ```
2. Create a file named .env under agents/google_adk.
    ```bash
    touch agents/google_adk/.env
    ```
3. Add `GOOGLE_API_KEY` to .env  (sample uses Google Gemini by default)

4. Run an agent:
    ```bash
    uv run google_adk/agent
    ```
5. Run one of the [client apps](/samples/python/hosts/README.md)
