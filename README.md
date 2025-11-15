# data-analyzer-ai-agent

## To run locally
 Create a .env file and add the below to it. Yoiu need to login with your azure account for authentication

 ```env
 PROJECT_ENDPOINT=""      # your por
MODEL_DEPLOYMENT_NAME="gpt-4o"
 ```

 your_project_endpoint placeholder with the endpoint for your project and ensure that the MODEL_DEPLOYMENT_NAME variable is set to your model deployment name (which should be gpt-4o).

---

### What this code is doing

- Connects to the AI Foundry project.
- Uploads the data file and creates a code interpreter tool that can access it.
- Creates a new agent that uses the code interpreter tool and has explicit instructions to use Python as necessary for statistical analysis.
- Runs a thread with a prompt message from the user along with the data to be analyzed.
- Checks the status of the run in case there's a failure
- Retrieves the messages from the completed thread and displays the last one sent by the agent.
- Displays the conversation history
- Deletes the agent and thread when they're no longer required.

---

## Summary

We have used the Azure AI Agent Service SDK to create a client application that uses an AI agent. The agent can use the built-in Code Interpreter tool to run dynamic Python code to perform statistical analyses.

---
