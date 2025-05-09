# Codebase Analysis and Documentation
 

You can use a tool like [repomix](https://github.com/yamadashy/repomix) to help streamline your codebase management.

Another option is to use an AI Agent with the following prompt:

```prompt
Please analyze the codebase and provide a summary of the following aspects:

## Technical Architecture
- **System Architecture**: Outline the high-level architecture of the 
  application/system, including components, services, and their relationships.

## Dependencies
- **Package Analysis**: List all dependencies with their versions from configuration 
  files (package.json, pyproject.toml, requirements.txt, Gemfile, etc.).
- **Third-party Integrations**: Identify external services or APIs integrated with 
  the system.
- **Development Dependencies**: Separate out testing, linting, and other 
  development-only packages.

## Documentation & Project Structure
- **Project Organization**: Map the directory structure with descriptions of key 
  folders and their purpose.
- **Technical Documentation**: Summarize existing documentation (README.md, docs/, 
  wikis, etc.), noting important setup instructions and guides.
- **Comments Quality**: Assess the quality and comprehensiveness of code comments 
  throughout the project.

## Code Quality & Patterns
- **Coding Conventions**: Identify coding standards, style guides, and linting 
  configurations.

Create a folder 'context' in the root of the repository and place the report in it.
Create this report in a file called `repo-spec.md` in the 'context' folder.
```

> **Recommended approach**: Based on practical experience, this shorter version is actually more effective. It provides a focused and more actionable overview of the codebase while requiring less processing time from the AI. For most projects, this concise prompt delivers better results and is the recommended option.

For more comprehensive analysis, you can use this alternative prompt:

```prompt
Please perform a comprehensive analysis of this repository to create a 
developer-friendly overview. Explore and identify the following key aspects:

## Technical Architecture
- **Main Technologies**: Identify all programming languages with their approximate 
 usage percentage, frameworks, libraries, and tools used throughout the codebase.
- **System Architecture**: Outline the high-level architecture of the 
 application/system, including components, services, and their relationships.
- **Build and Deployment**: Analyze the build pipeline, deployment configurations, 
 and environment setup (Docker, CI/CD, etc.).

## Dependencies
- **Package Analysis**: List all dependencies with their versions from configuration 
 files (package.json, pyproject.toml, requirements.txt, Gemfile, etc.).
- **Third-party Integrations**: Identify external services or APIs integrated with 
 the system.
- **Development Dependencies**: Separate out testing, linting, and other 
 development-only packages.

## Documentation & Project Structure
- **Project Organization**: Map the directory structure with descriptions of key 
 folders and their purpose.
- **Technical Documentation**: Summarize existing documentation (README.md, docs/, 
 wikis, etc.), noting important setup instructions and guides.
- **Comments Quality**: Assess the quality and comprehensiveness of code comments 
 throughout the project.

## Code Quality & Patterns
- **Coding Conventions**: Identify coding standards, style guides, and linting 
 configurations.
- **Design Patterns**: Recognize common design patterns implemented in the codebase.
- **Testing Approach**: Evaluate the testing strategy, coverage, and types of tests 
 (unit, integration, e2e).

## APIs & Data Models
- **API Endpoints**: Document all API endpoints, their request/response formats, 
 authentication methods, and protocols.
- **Data Models**: Identify key data structures, schemas, and their relationships.
- **State Management**: Analyze how application state is managed (if applicable).

## Performance & Security
- **Performance Considerations**: Note any performance optimizations or concerns.
- **Security Mechanisms**: Identify authentication, authorization methods, and other 
 security practices.

## Developer Experience
- **Development Setup**: Summarize the steps required to set up the development 
 environment.
- **Common Workflows**: Identify common development workflows (build, test, deploy).

Create a folder 'context' in the root of the repository and place the report in it.
Create this report in a file called `repo-spec.md` in the 'context' folder.
```

 