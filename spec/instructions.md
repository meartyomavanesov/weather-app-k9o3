**Critical Rules**
- DO NOT change the architecture or structure unless EXPLICITLY instructed.
- DO NOT introduce new major dependencies without EXPLICIT approval.
- DO NOT remove or significantly refactor existing code unless DIRECTLY required for the task.
- DO NOT remove or break existing functionality unless EXPLICITLY instructed.

**Implementation Guidelines**

**General Approach**
- Changes should be minimal and focused.
- Only modify what is absolutely necessary to fulfill the requirement and nothing else.
- Implement only the base minimum to meet the requirement and nothing beyond what is necessary.
- Do not come up with new requirements that are not specified.

**Reuse & Modularity**
- Re-use existing components, patterns, configurations, and standards when possible.
- Only introduce new ones when it is impossible to fulfill the requirement with existing ones.
- New components and other additions should be isolated and modular so they are easy to adjust or remove without touching other areas of the application.

**Testing & Cleanup**
- Ensure the implementation is immediately testable and use mock data if real data is not available.
- After refactoring, clean up any code that is not needed anymore following the change while ensuring everything continues to work as intended and nothing breaks.
- After major refactoring, review parts of the code base related to the changed parts and make sure that they remain integrated, functioning, stable, and up-to-date.

**User Guidance & Security**
- If user action is required to complete a task (e.g. connecting or configuring an external service), provide clear step-by-step instruction to the user and guide them through the process.
- Make sure that secrets and keys are handled securely. Prioritize security.
- When a new dependency is introduced, explain why the dependency is needed to the user and request permission from the user to install it.
- Do not install dependencies without explicit approval.

**Architecture & Logic**
- Ensure that core and critical logic is handled in the back-end.
- At the same time, make sure the back-end footprint is small so that it is easy to understand, maintain, and debug.

**Documentation & Communication**
- Add, update, or remove comments where necessary.
- Clearly communicate what was built and why.