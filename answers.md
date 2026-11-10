# MCP Assignment Answers

### 1. How many tools were available in Part 1 and Part 3? What changes were required in the client?

Initially, the MCP server provided 8 tools in Part 1. After implementing the new `predict_both` function, the server provided 9 tools in Part 3. The client automatically detected the additional tool through `list_tools()`. A separate client script (`my_client.py`) was created to access and test the new functionality.

### 2. For how many test patients did the models produce different predictions? Which model made the correct prediction?

The two models gave different predictions for 8 of the 114 test patients.

- Patient 3: Logistic Regression predicted correctly.
- Patient 25: Logistic Regression predicted correctly.
- Patient 48: Logistic Regression predicted correctly.
- Patient 53: KNN predicted correctly.
- Patient 76: Logistic Regression predicted correctly.
- Patient 80: Logistic Regression predicted correctly.
- Patient 99: Logistic Regression predicted correctly.
- Patient 102: Logistic Regression predicted correctly.

### 3. Which model performed better in the cases where their predictions differed?

Logistic Regression performed better in these cases. It correctly classified 7 of the 8 patients, whereas KNN correctly classified only 1 patient.

### 4. What is the importance of the triple-quoted tool description for an AI application?

The description tells the AI application the purpose of the tool and explains its functionality. This helps the AI understand when the tool is appropriate to use and how it can help answer a request.

### 5. Why should an MCP server maintain a record of every tool call?

Maintaining tool-call records makes it easier to monitor server activity, identify failed operations, troubleshoot problems, and review previous requests. These records also help ensure transparency and accountability.