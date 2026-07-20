# Final Project: LLM-Powered Research Planning Agent

## Objective
The objective of the final project was to design, implement and critically evaluate an intelligent multi-agent system capable of assisting users with academic research. The project was completed in two phases. During Week 7, a comprehensive multi-agent architecture was collaboratively designed to support literature discovery, evidence analysis and report generation. During Week b11, this design informed the implementation of a working prototype that demonstrated the core functionality of an LLM-powered research planning agent.


## Project Overview
Academic research requires significant time top identify relevent literature, evaluate source credibility, sythesis findings and organise information into meaningful summaries (Wooldridge, 2009). The aim of this project was to investigate how intelligent agents and Large Language Model (LLMs) could automate parts of this process while maintaining transperancy and structured decision-making.

The completed prototype accepts the research topic from the user, general reads a research plan, retrieve relevant academic literature and produces a structured research summary.

## Week 7: System Design
The initial system design was developed collaboratively as part of the group project. The propose architecture consisted of multiple specialised agents working together under a supervisor architecture (Arsanjani and Bustos, 2026). Rather than allowing autonomous agents to make uncontrolled decisions, the Supervisor Agent coordinted task execution, ensuring that the research process remained transparent, auditable and explainable (Arsanjani and Bustos, 2026).

The proposed system included specialised agents respionsible for source retrieval, document parsing, summarisation, credibility assessment, contradiction detection, hypothesis extraction, evidence linking, convergence analysis and report publishing. Communication between these agents was facilitated using A2A-style messaging and a blackboard knowledge hub, allowing agents to exchange information while maintaining a shared representation of the current research task (Wooldridge, 2009).

The key design decision was the use of static task registry instead of dynamically generated tasks. This improved system reliability, explainability and auditability by ensuring that each agent operated within predefined responsibilities. The architecture also incorporated both short-term memory(blackboard knowledge hub) and long-term memory (vector database) to support knowledge reuse and continuity across research tasks.


## Week 11: System Implementation
The week 11 implementation trabsalted the conceptual design into a functional prototype using python. While the complete multi-agent architecture proposed during the week 7 was beyond the scope of the individual implementation, the prototype successfully demonstrated the core resarch planning workflow.

The implemented system consisted of several key components:

- Planner agent
- retrieval agent
- processing agent
- research summary generator
- GitHub-based projector repositary
- LLM integration for research planning and summarisation

The prototype accepts the research topic from the user and generates a structured research plan before retrieving relevant academic papers. The retrieved information is then processed and organised into a concise research summary, demonstrating the interaction between multiple software components to support academic literature (Lewis et al., 2020).

### Comparison Between Design and Implementation

The implemented prototype successfully achieved the primary objective of demonstrating an intelligent research planning workflow. However, several advanced features propose during the design phase were intentionally simplified.

The original architecture proposed specialised agents for contradiction detection, credibility scoring, hypothesis extraction, convergence analysis and long-term memory management. Due to project scope and implementation time constraints, the individual prototype focused on implementing the essential planning, retrieval and summarisation pipeline.

Although simplified, implementation preserved the overall architectural philosophy developed during the design phase by maintaining modular components that could be extended into a complete multi-agent system (Arsanjani and Bustos, 2026).


### Testing and Evaluation
The completed prototype was tested using multiple research topics to evaluate its ability to generate research plans and produce meaningfull summaries.

Testing demonstrated that the system was capable of:

- accepting user research topics
- Generating structured research plans
- receiving relevant academic literature
- Producing coherent research summaries
- demonstrating the interaction between intelligent software components

The modular implementation also allowed each component to be tested independently, making debugging and future extension significantly easier  (Yao et al., 2023).

## Critical Evaluation
The project successfully demonstrated how intelligent agents and large language models can support academic research by automating repetitive information gathering and summarisation tasks (Lewis et al., 2020).

One of the greatest strengths of the system was it modular architecture. Separating responsibilities into specialised components improved maintainability, readability and future scalability. The design also emphasised explainability by encouraging usable decision-making rather than rely on a single monolithic AI Model (Yao et al., 2023).

However, the implementation also highlighted several limitations. The prototype did not fully implement all of the specialised agents proposed during the design stage, particularly those responsible for contradiction detection, credibility assessment and convergence analysis. Additionally, the quality of generated summaries remained dependent on the capabilities of the underlying large language model and the quality of retrieved research sources (Lewis et al., 2020).

Future improvements could include implementing the remaining specialised agents, integrating a persistent vectors for long-term memory, expanding support for additional academic databases and introducing explainable AI techniques to improve user trust in generated outputs (Arsanjani and Bustos, 2026).

## Skills Developed
This project strengthened both my technical and professional skills, including:

- Multi-agent system design
- intelligent agent architectures
- large language model integration
- Python software development
- Git and GitHub version control
- research planning and system evaluation
- critical thinking and problem-solving
- reflective software engineering

## Reflection

This project demonstrated the practical challenges involved in transforming a conceptual multi-agent architecture into a working software prototype (Wooldridge, 2009). Throughout the development process, I gained a greater appreciation for the importance of modular systems design, explainability and iterative software development.

Comparing the original architecture with the final iplementation showed the software engineering often requires balancing ambitious design goals with practical development constraints. Rather than attempting to implement every proposed feature, I prioritised the core functionality required to demonstrate the intelligent research planning workflow (Arsanjani and Bustos, 2026).this experience reinforced the value of incremental development and highlighted opportunities for future enhancement.

## References
Arsanjani, A. and Bustos, J.P. (2026) Agentic Architectural Patterns for Building Multi-Agent Systems. Birmingham: Packt Publishing.

Lewis, P., Perez, E., Piktus, A., Petroni, F., Karpukhin, V., Goyal, N., Küttler, H., Lewis, M., Yih, W.T., Rocktäschel, T. and Riedel, S. (2020) 'Retrieval-augmented generation for knowledge-intensive NLP tasks', Advances in Neural Information Processing Systems, 33, pp. 9459-9474.

Wooldridge, M. (2009) An Introduction to MultiAgent Systems. 2nd edn. Chichester: John Wiley & Sons.

Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K. and Cao, Y. (2023) 'ReAct: synergizing reasoning and acting in language models', arXiv preprint, arXiv:2210.03629.