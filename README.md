# Chatbot Using LangGraph
This project demonstrates how to create a chatbot using the `langgraph` framework. The chatbot is designed to process messages and generate appropriate responses by utilizing state transitions within a conversation graph.
# Key Components
1. **Importing Required Modules**:
   The code imports necessary modules from the `langgraph` library, including:
2. **Defining the State**:
   A state is defined using Python’s `TypedDict`, where the `messages` key holds a list of messages in the conversation. The `add_messages` function ensures new messages are appended to the list instead of replacing previous ones.
3. **Creating the Conversation Graph**:
   A `StateGraph` object is created, which will serve as the framework for managing states in the chatbot's conversation flow.
4. **Chatbot Function**:
   The chatbot function takes the current state of the conversation (a dictionary of messages) and uses the `llm.invoke` method to generate a response based on the incoming messages. This function will be linked to the conversation graph.
5. **Adding Nodes to the Graph**:
   The `chatbot` function is added as a node to the conversation graph, making it an interactive part of the state transitions in the chatbot system.
6. **Running the Chatbot**:
   To run the chatbot, you will need to execute the notebook cells and interact with the chatbot via the conversation graph. The chatbot is designed to handle a series of incoming messages and generate responses accordingly.
