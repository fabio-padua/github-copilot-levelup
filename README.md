# GitHub Copilot Level Up

This repository is a playground for **leveling up with GitHub Copilot** using two complementary approaches:

1. **Prompt files**: reusable, version-controlled instructions that help Copilot generate consistent results.
2. **Vibe coding**: iterating quickly by describing intent, testing small slices, and letting Copilot fill in the implementation.

The goal is to create **cool apps faster**, while keeping a clear record of the prompts and patterns that worked.

## What you'll find here

- A place to store prompt files (for example in a `prompts/` folder)
- Small experiments and app prototypes generated with Copilot
- Notes and examples showing how to run Copilot effectively

## Using prompt files with GitHub Copilot

Prompt files (often written in Markdown) let you capture:

- project context
- architecture constraints
- preferred libraries / frameworks
- coding standards
- test expectations

### Example prompt file

Create a file such as `prompts/new-app.md`:

```markdown
# New App Prompt

You are building a small web app.

Requirements:
- Use TypeScript
- Provide a minimal REST API
- Include unit tests

Output:
- Explain the file structure
- Provide the code
```

Then open that file in your editor and ask Copilot to generate code based on it.

## Vibe coding workflow (recommended)

A simple loop:

1. Describe the next tiny step ("Add a health check endpoint")
2. Let Copilot propose code
3. Run tests / lint / app
4. Adjust the prompt and iterate

This keeps momentum while staying in control.

## How to execute this with GitHub Copilot (samples)

### Sample 1: Create a new prototype from scratch

1. Open the repository in **VS Code**.
2. Open **Copilot Chat**.
3. Ask:

   "Create a simple TODO API using Node.js + Express + TypeScript. Include Dockerfile and tests." 

4. When Copilot suggests files, accept changes.
5. Run:

   ```bash
   npm install
   npm test
   npm run dev
   ```

### Sample 2: Use a prompt file to guide generation

1. Create a prompt file: `prompts/todo-api.md` describing requirements and constraints.
2. In Copilot Chat, ask:

   "Read `prompts/todo-api.md` and generate the initial project structure and code. Keep it minimal." 

3. Iterate:

   "Now add request validation and error handling." 

### Sample 3: Refactor with Copilot

- Select a file in VS Code.
- In Copilot Chat ask:

  "Refactor this to use a service layer and add unit tests. Keep behavior the same." 

## Contributing

This repo is intentionally experimental. Feel free to add:

- new prompt files that worked well
- small app ideas and prototypes
- notes about Copilot usage

## License

MIT