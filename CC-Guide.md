# Guide to using Claude Code

> The Less Ambiguity, the Better
> Be Thorough and Precise: Early
> The Better your English, the Better your Code
> Understand the inputs and the outputs: let Claude do the rest

## Development Stages

1. **Preparation** - Define the feature
2. **Research** - Gather information (optional)
3. **Planning** - Create implementation plan
4. **Implementation** - Execute the plan
5. **Testing** - Verify functionality
6. **Documentation** - Update documentation
7. **Verification** - Review changes (optional)

## Stage Details

### Preparation

Rigorously describe the feature (e.g., bug fix or enhancement) that you want to implement.

- Consider what background information, resources, and code will be relevant for this feature
- Refrain from using Claude for this stage
- If you'd like to learn about a concept relevant to your feature, feel free to use AI to assist you

### Research (Optional)

Instruct Claude to perform web searches for documentation, code examples, background information, etc.

- Ensure that Claude is searching for documentation that corresponds to the package versions you are using
- Enable **thinking** during this phase

### Planning

If you have not already presented your feature to Claude, do it now.

- Instruct Claude to develop a "concise and high level" plan document (a markdown file)
- Ensure that the plan aligns with your intentions before continuing
- Instruct Claude to ask you "clarifying questions" regarding your request(s)
- Enable **thinking** during this phase
- Note: After planning is completed, you may want to **compact** the conversation (e.g., "/compact Prepare for implementation of the plan")

### Implementation

Instruct Claude to systematically work through the plan.

- Inform Claude to verify proper typing throughout development (e.g., "Use `uv run pyright` throughout the implementation process.")
- You may wish to instruct Claude to apply formatting and linting actions throughout implementation
- You may disable **thinking** during implementation, though it may be desirable for particular stages
- Consider setting **accept edits on** when Claude is on the right track, but monitor its progress
- You may wish to **compact** throughout and after implementation

### Testing

After Claude has finished implementation:

- Instruct Claude to create tests for new changes and run them
- Have Claude perform a demo run of the application (e.g., "Perform a dry run of the program"), if applicable
- Ensure proper typing, linting, formatting, etc., either with Claude or manually

### Documentation

Instruct Claude to update the documentation, primarily the CLAUDE.md memory file, before committing changes.

- Use custom commands to enforce standards for Claude's memory files (if available)

### Verification (Optional)

After the feature is fully implemented, tested, and documented:

- Have another instance of Claude thoroughly analyze recent changes
- Instruct it to look for "bugs, potential bugs, logical issues, and potential logical issues"

## General Tips

### Autonomous Development

To take advantage of autonomous development (i.e., "accept edits on"):

- Develop programs that facilitate demo runs (e.g. develop scripts to run your program locally)
- Include a "dry run" flag in programs to run simplified versions
- Note: Demo runs don't guarantee successful execution in all environments without extensive development, but they are verifiable.

### Feature Scope

- Keep features to an appropriate size—learn the right scope through experience
- Even with extensive research and planning, Claude will likely overlook some facets
- Start with smaller, well-defined features to minimize oversight



