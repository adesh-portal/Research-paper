# AI Human Capital & the Future of Work
## A Privacy-Preserving Local Personal AI Assistant

A local-first personal AI assistant designed to run AI inference directly on the user's device, reducing reliance on cloud services and keeping personal data under the user's control.

## Project Overview

This project proposes a privacy-preserving AI assistant that uses an on-device large language model (LLM), such as a model served through Ollama, to support everyday productivity tasks. Its local-first approach aims to enable useful AI functionality without sending sensitive user data to external servers.

The proposed assistant focuses on:
- Local AI inference and offline operation
- Smart search across local files
- Document reading and summarization
- Notes organization and quick actions
- Workflow automation for routine tasks
- Local data storage, access control, and privacy

## Problem Statement

Cloud-based AI assistants may require user inputs to be transmitted to remote servers for processing. This can introduce privacy and data-ownership concerns, dependence on a stable internet connection, network-related latency, and potential exposure through third-party storage or services.

## Objectives

- Keep processing and storage on the user's device wherever supported.
- Provide AI functionality when an internet connection is unavailable.
- Help users find local files using natural-language queries.
- Summarize documents into concise, useful key points.
- Organize notes and support productivity-oriented quick actions.
- Automate selected repetitive tasks.
- Protect locally stored information through appropriate security controls.
- Use device resources efficiently, including through model optimization where applicable.

## Core Features

### 1. Smart File Search
Search local documents and files using natural-language queries, with relevance-based results and filters such as file type or date where implemented.

### 2. Document Summarization
Read supported documents and produce concise summaries of their main ideas. The research paper describes TXT, DOCX, and PDF as intended formats; actual support depends on the implementation.

### 3. Notes Organization
Create, edit, categorize, and retrieve notes. Planned quick actions include tags, to-do lists, reminders, and study-related organization.

### 4. Workflow Automation
Support selected repetitive tasks, such as organizing files and scheduling reminders, according to user-defined rules and the capabilities implemented in the application.

### 5. Offline Inference
Run the language model locally so that supported AI operations can work without sending prompts to a cloud model. Initial model setup or downloads may still require internet access.

## Proposed Architecture

The research describes four layers:

1. **Local Model Layer** — hosts the local language model and performs inference.
2. **Task Management Layer** — interprets requests and routes them to the appropriate functional module.
3. **User Interface Layer** — provides the interaction experience, such as chat and quick actions.
4. **Storage & Security Layer** — manages local data, access control, and protection mechanisms.

## Technology Direction

- **Local LLM runtime:** Ollama is identified in the research as an example for local inference.
- **Model optimization:** Quantization and pruning are proposed as possible ways to reduce resource use.
- **Local processing:** Input preprocessing, model inference, and output postprocessing are intended to run on the device.
- **Security:** Local storage, authentication, and encryption are design goals; the level of protection depends on what is implemented in the application.

The available project materials describe the intended system and architecture. They do not specify a complete, verified installation procedure, exact dependency versions, or the current implementation status of every feature.

## Privacy Design

The intended design is local-first: personal data should remain on the user's device and should not be sent to external AI services during local inference. For a real deployment, verify that telemetry, logging, model downloads, integrations, and other network features do not transmit sensitive information. Apply suitable access controls and encryption to stored data.

## Potential Use Cases

- **Education:** Summarize study material and organize notes.
- **Personal productivity:** Find files, manage notes, and set reminders.
- **Office work:** Search documents and summarize reports.
- **Privacy-sensitive workflows:** Process information locally where appropriate.
- **Limited-connectivity environments:** Use supported features without an active internet connection.

## Future Scope

The research proposes several possible extensions:
- Model optimization through quantization and pruning
- Desktop and mobile platform support
- Offline voice recognition
- Real-time translation and additional offline AI features

These are future directions, not guarantees that the features are already implemented.

## Evaluation

The research identifies response latency, memory use, task success, summary relevance, reliability, and user experience as evaluation areas. Claims such as a specific speed improvement or complete privacy should be validated through reproducible tests on the target hardware before being treated as measured results.

## Project Contributors

- Prachi Sahu
- Anshika Singh
- Adesh Trivedi

**Guide:** Mr. Deepak Kumar Singh  
**Institute:** Allenhouse Business School, Kanpur

## Current Status and Contributions

This README summarizes the project's concept and proposed design based on the provided research materials. Update this section with the actual implementation status, screenshots, supported file types, model name, hardware requirements, and test results before publishing the repository.

## License

No license was specified in the provided project materials. Add a license file if you intend to distribute the source code publicly.
