# Create an Implementation Plan

Your task is to create a comprehensive implementation plan from a design document. Transform the provided design document into a detailed, actionable task list formatted as `tasks.md`.

## Input:

You will receive:
- a design document discribing the system (or parts of) to be implemented
- the requirements in BDD format used to create the design document  

## Requirements:

### Task Structure:
1. **Main Tasks**: Number each main task (1, 2, 3, etc.) with a checkbox `- [ ]`
2. **Subtasks**: Use decimal notation (2.1, 2.2) for subtasks, also with checkboxes  
3. **Task Descriptions**: Write clear, specific, actionable descriptions  
4. **Technical Details**: Include specific technical details from the design (e.g., API names, data models, thresholds)  
5. **Requirements Tracking**: End each task/subtask with _Requirements: X.X, Y.Y_ mapping to the original requirement number  

### Task Organization:
1. **Setup & Foundation**: Start with data models, schemas, and core infrastructure  
2. **Core Implementation**: Build services, APIs, and main functionality  
3. **UI Components**: Create user interface elements  
4. **Integration**: Connect all components together  
5. **Testing**: Add comprehensive test coverage  
6. **Optimization**: Performance improvements and monitoring  
7. **Deployment**: Configuration and rollout  

### Task Writing Guidelines:
- Use imperative mood ("Create", "Implement", "Update")  
- Be specific about what needs to be done  
- Include technical specifications from the design 
- Break complex features into manageable subtasks  
- Ensure logical dependencies (foundational work before dependent features)  
- Include error handling, fallback strategies, and edge cases  
- Reference specific interfaces, classes, and functions from the design  

### Content Extraction:
- Pull all technical specifications (thresholds, limits, model names)  
- Include all data models and interfaces mentioned  
- Capture all API integrations and external services  
- Include security, performance, and monitoring requirements  
- Don’t skip error handling and fallback strategies  

### Format Example:
```markdown
# Implementation Plan

- [ ] 1. Set up core data models and database schema  
  - Create TypeScript interfaces for [specific models]  
  - Add [specific field] to existing [interface]  
  - Create database migration scripts for [database] schema updates  
  - _Requirements: 1.1, 4.1, 7.1_  

- [ ] 2. Enhance [specific API] integration  
  - [ ] 2.1 Update API response interface  
    - Modify existing [interface] to include [field]  
    - Update parsing to extract [information]  
    - _Requirements: 4.1, 4.2_  
```

### Special Instructions:
- Ensure 100% coverage of design features  
- Maintain consistency with existing system architecture  
- Include both frontend and backend tasks  
- Consider offline functionality and synchronization  
- Include configuration and feature flag setup  
- Add comprehensive testing at unit, integration, and UI levels  
- Include performance optimization tasks  
- Don’t forget monitoring, logging, and alerting setup  

---

Transform the design document into a complete, professional implementation plan that a development team can execute sequentially. Output the resulting tasks in a new tasks.md file in the same directory as its design.md.

<design__file>
$ARGUMENTS
<\design_file>