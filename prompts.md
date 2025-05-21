**Suggested prompts for each iteration & MCP Configuration**

## Iteration 1 - Prompt

```
Using the iteration-1 folder, read the requirements.md attentively and implement what is being asked.
```

## Iteration 2 - Prompt

```
Using the iteration-2 folder, read the requirements.md attentively and implement what is being asked.
```

## Iteration 3 - Prompt

```
Using the iteration-3 folder, read the requirements.md attentively and break down the implementation into tasks using a tasks.md file - you MUST fully cover all requirements. The task's list should be placed under a markdown table, containing the following columns: ID, Task Description, Notes, Depends on, Status.

Guidelines:

(1) Before start the implementation, ask for user confirmation on the tasks.md file created.
(2) Use the Notes column in the tasks.md file to add any complementary notes from requirements.md in order to provide correct and full coverage of all requirements.
(3) Use the Status column in the tasks.md file to track the progress of each task once it's completed.
(4) Once a task is completed, commit changes - use the commit message "Task ID: Task Description"
```

## Testing with Playwright MCP

### Configuration

First, let's configure the Playwright MCP on Windsurf:
    - Windsurf Settings / Cascade / Model Context Protocol (MCP) Servers / Add Server / Select "Playwright" in the list
    - Update the mcp_config.json file > add the "--vision" param to the playwright args

### Prompt 1

```
Use the playwright mcp to run the test scenario in iteration-3/3d-game.feature.
```

### Prompt 2

```
Use the playwright mcp to run the test scenario in iteration-3/3d-game.feature and:

1. Provide a test report
2. Record all successful mcp tool calls into an md file - use the scenario id as the file name
3. Create a pageObject file with all html elements (xpath) used within the successful mcp tool calls
```