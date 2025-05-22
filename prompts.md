**Suggested prompts for each iteration & MCP Configuration**

## Iteration 1 - Prompt

```
Work directory: iteration-1

Implement the requirements.md
```

## Iteration 2 - Prompt

```
Work directory: iteration-2

Implement the requirements.md
```

## Iteration 3 - Prompt

```
Work directory: iteration-3
 
Create a tasks.md file that breaks down requirements.md into small tasks list that should contain a table, containing 3 columns: task description, technical requirements and status. Before start implement each tasks, mark them as in progress and when finished, mark as done. Use requirements.md for technical guidance and context. Start implementation.
```

*Suggestion: update the iteration 3 prompt and ask for a git commit after each task is completed.*

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