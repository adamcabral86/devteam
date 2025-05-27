---
description: 
globs: 
alwaysApply: true
---
You are an AI agent participating in a collaborative software development project. Your actions are governed by a set of rules and your individual agent profile. To perform your tasks effectively, you need to access information from several files within the project directory. Please follow these instructions carefully:

1.  File Locations:

devteam/
├── agentrules.mdc               # Agent rules document
├── Context/
│   ├── active_context.md          # Active context file
│   ├── progress.md                # Progress tracking file
│   └── team_context.md            # Team communication history 
├── Team/
│   ├── rules.md                   # Team rules document
│   └── agent_profiles.json        # Agent profiles and configurations
|   └── improvement_suggestions.md # Agent suggestions for rule/profile improvements (All Agents)
└── PRD/
    │   prd.md                     # Main Product Requirements Document.
    │                              # Contains the overall requirements, goals, user stories,
    │                              # and high-level specifications for the project.
    │                              # It is authored and maintained by Emma (Product Manager).
    │                              # Format: Markdown.
    │   class_diagram.md           # Class diagram for the system.
    │                              # Depicts the classes, their attributes, and relationships.
    │                              # It is authored and maintained by Bob (System Architect).
    │                              # Format: Markdown, includes Mermaid code for rendering.
    │   sequence_diagram.md        # Sequence diagrams for key workflows.
    │                              # Illustrates the interactions between different parts of the system
    │                              # for specific use cases.
    │                              # It is authored and maintained by Bob (System Architect).
    │                              # Format: Markdown, includes Mermaid code for rendering.

    * Rules Document: The core rules governing your behavior and communication are located in the file named `devteam/rules.md`. You **MUST** read and understand this file before processing any other information.
    * Team Context: All project communication, task assignments, progress updates, and the ongoing conversation history are stored in the file named `Context/team_context.md`. You **MUST** refer to this file to understand your current tasks, the project's status, and any relevant information.
    * Agent Profiles: Your individual agent profile, which details your role, capabilities, and specific interaction protocols, is located within the file named `devteam/agent_profiles.json`. You **MUST** read and understand your profile to act correctly.

2.  Processing Order:

    * PRIORITY 1: Read `devteam/rules.md`
        * Begin by opening and thoroughly reading the entire content of the `devteam/rules.md` file.
        * Internalize the rules and guidelines provided in this file. These rules are essential for proper behavior and communication.
        * If there are any conflicting instructions, the `devteam/rules.md` document takes precedence.

    * PRIORITY 2: Read `devteam/agent_profiles.json`
        * Open and read the entire content of the `devteam/agent_profiles.json` file.
        * Identify your agent profile by matching the "agent_name" field to your assigned agent name.
        * Pay close attention to your profile's `role_description`, `core_capabilities`, and `interaction_protocols`. These define how you should act.
        * If you are 'Milke', carefully review the `agent_registry` in your profile as it's crucial for task delegation.

    * PRIORITY 3: Read `Context/team_context.md`
        * Open and read the `Context/team_context.md` file.
        * Identify entries that are relevant to you:
            * If you are writing to the file, append your new entry to the end.
            * If you are reading the file, focus on new entries since your last check (if you can track this). Look for entries addressed to you (e.g., `@YourAgentName:`) or general project updates.
            * Pay attention to timestamps to maintain chronological order.

3.  Important Considerations:

    * File Integrity: Do not modify the file names or paths. Assume they are always accessible as specified.
    * Complete Reading: You **MUST** read the entire content of each file to avoid missing critical information.
    * Contextual Awareness: Maintain context across interactions. Remember previous tasks, decisions, and discussions.
    * Adherence to Rules: Always prioritize the rules outlined in `devteam/rules.md`.
    * Profile Compliance: Strictly adhere to the instructions and protocols defined in your `devteam/agent_profiles.json`.
    * Clear Communication: When writing to `Context/team_context.md`, be clear, concise, and use the specified format (e.g., `[Timestamp] YourAgentName: Message`).

By following these enhanced instructions, you will ensure that you correctly access and utilize the information within the provided files, leading to more effective collaboration and task execution.