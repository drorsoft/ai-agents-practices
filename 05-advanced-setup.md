# Advance setup

Different agents use different setups.  

## For all agents

To help AI agents better understand your repository and write code effectively, include these key Markdown files:

### Essential Documentation Files

1. **README.md**
   - Overview of the project
   - Purpose and main features
   - Installation instructions
   - Quick start guide
   - Basic usage examples
   - Links to more detailed documentation

3. **CONTRIBUTING.md**
   - Code style guidelines
   - Commit message format
   - Pull request process
   - Development environment setup
   - Testing requirements
   - Branch naming conventions
   - Code review process and expectations
   - Documentation requirements
   - AI-friendly code patterns
   - Project-specific linting rules
   - Component creation guidelines
   - Dependencies management policy
   - Performance and accessibility standards
   - Security requirements for contributions
   - Versioning guidelines

## Copilot

For GitHub Copilot specifically, add:

1. **Repository Custom Instructions (`.github/copilot-instructions.md`)**
   - Creates repository-wide instructions that apply to all Copilot Chat conversations
   - Allows you to provide project-specific context without repeating it in every prompt
   - Helps tailor AI responses to your team's workflow, tools, and project specifics
   - Example instructions can include:
     - Coding style preferences (e.g., "We always write JavaScript with double quotes and tabs for indentation")
     - Build tool preferences (e.g., "We use Bazel for managing Java dependencies, not Maven")
     - Project management information (e.g., "Our team uses Jira for tracking work items")

2. **Prompt Files (VS Code only, `.github/prompts/*.prompt.md`)**
   - Creates reusable prompt instructions for specific tasks
   - Can reference other workspace files to provide additional context
   - Great for standardizing common AI-assisted tasks
   - Example use cases:
     - Component generation templates
     - Code review checklists
     - Security review guidelines
 

 ## Cursor

For Cursor AI specifically, add:

1. **Project Rules (`.cursor/rules/*.mdc`)**
   - Stored in version-controlled `.cursor/rules` directory
   - Written in MDC format with support for metadata and content
   - Scoped to your codebase for project-specific instructions
   - Rule types include:
     - Always: Always included in the model context
     - Auto Attached: Included when files matching a glob pattern are referenced
     - Agent Requested: Available to the AI, which decides whether to include it
     - Manual: Only included when explicitly mentioned using @ruleName
   - Example use cases:
     - Domain-specific knowledge about your codebase
     - Project architecture standards
     - Style guidelines and best practices
     - Workflow automation templates

2. **User Rules (Cursor Settings > Rules)**
   - Global to your Cursor environment
   - Always applied across all projects
   - Written in plain text (no MDC support)
   - Example use cases:
     - Setting response language or tone
     - Personal style preferences
     - Consistent AI behavior across projects

3. **Legacy `.cursorrules` File**
   - Still supported but deprecated
   - Single file in project root
   - Being replaced by the more flexible Project Rules
   
### Creating Rules in Cursor

You can create rules through:
- Using `Cmd + Shift + P` > "New Cursor Rule"
- Going to `Cursor Settings > Rules`
- Using the `/Generate Cursor Rules` command in a conversation

### Best Practices for Rules

- Keep rules concise (under 500 lines)
- Split large concepts into multiple, composable rules
- Provide concrete examples or reference files when helpful
- Write rules as you would write clear internal documentation
- Reference other files using `@filename.extension` syntax

## Claude