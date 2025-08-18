# Create A Design Document

Your task is to transform a BDD requirements document into a comprehensive technical design document (`design.md`).

## Input Context

You will receive:
1. A requirements document with user stories and acceptance criteria  
2. (Optional) Other existing design documents from the system for integration context  

## Output Requirements

Create a professional design document with the following structure and characteristics:

### 1. **Overview Section**
- Provide a concise executive summary of the feature/system  
- Highlight the key business value and technical approach  
- Mention main technologies and integration points  
- Keep it to 1–2 paragraphs  

### 2. **Architecture Section**
- Include a high-level architecture diagram using Mermaid syntax  
- Show all major components, data flows, and external dependencies  
- Use appropriate diagram types (flowchart, sequence, component diagrams)  
- Explain the data flow in numbered steps  
- Include both frontend and backend components if applicable  

### 3. **Components and Interfaces Section**
- Define all core data models with TypeScript/appropriate language interfaces  
- Specify service interfaces and API contracts  
- Include request/response models  
- Add detailed field descriptions and constraints  
- Organize by logical groupings (Core Models, Service Interfaces, UI Components, etc.)  

### 4. **Data Models Section**
- Provide complete database schema designs  
- Include both SQL and NoSQL schemas if applicable  
- Define indexes, relationships, and constraints  
- Add migration considerations if updating existing schemas  
- Include both cloud and local storage schemas if relevant  

### 5. **AI/ML Integration Design** (if applicable)
- Detail prompt engineering approaches  
- Include example prompts and expected responses  
- Define model selection criteria and parameters  
- Add response processing logic with code examples  

### 6. **Error Handling Section**
- Enumerate all error categories  
- Provide specific recovery strategies for each error type  
- Include fallback mechanisms with implementation code  
- Add retry logic and circuit breaker patterns  

### 7. **Testing Strategy Section**
- Define unit, integration, and performance test scenarios  
- Include specific test cases aligned with acceptance criteria  
- Add code examples for key test implementations  
- Cover edge cases and failure scenarios  

### 8. **Security Considerations Section**
- Address API security (authentication, authorization, rate limiting)  
- Include data privacy and protection measures  
- Define encryption and data sanitization approaches  
- Add compliance considerations if applicable  

### 9. **Performance Optimization Section**
- Separate frontend and backend optimizations  
- Include caching strategies  
- Define batching and pagination approaches  
- Add specific performance targets and monitoring  

### 10. **Deployment Configuration Section**
- Define feature flags and rollout strategies  
- Include environment-specific configurations  
- Add monitoring and alerting setup  
- Define logging strategies and retention policies  

## Design Principles to Follow
1. **Technical Depth**: Provide implementation-ready details with code snippets  
2. **Scalability Focus**: Design for growth and high availability  
3. **Error Resilience**: Include comprehensive error handling and recovery  
4. **Performance First**: Optimize for speed and efficiency from the start  
5. **Security by Design**: Embed security considerations throughout  
6. **Testability**: Ensure all components are easily testable  
7. **Maintainability**: Use clear naming, documentation, and modular design  

## Code Style Guidelines
- Use TypeScript for frontend/Node.js code examples  
- Use Python for AI/ML and backend processing examples  
- Use SQL for database schemas  
- Use Mermaid for all diagrams  
- Include comprehensive type definitions  
- Add comments for complex logic  

## Quality Checklist
- [ ] Every acceptance criteria maps to a technical implementation  
- [ ] All external dependencies are identified and documented  
- [ ] Error scenarios have defined handling strategies  
- [ ] Performance requirements have specific optimization strategies  
- [ ] Security measures address all data flows  
- [ ] Testing strategy covers all critical paths  
- [ ] Deployment strategy includes rollback procedures  

## Special Considerations
1. **For AI/ML Features**: Include prompt engineering, model selection, token optimization, and response validation  
2. **For Real-time Features**: Address websocket/polling strategies, state synchronization, and conflict resolution  
3. **For Mobile Features**: Consider offline functionality, battery optimization, and platform-specific implementations  
4. **For Data-Heavy Features**: Include pagination, lazy loading, and data compression strategies  

---

Transform the requirements into a design document that a development team can immediately use to begin implementation. Be specific, technical, and comprehensive while maintaining clarity and good organization. Output the resulting design in a new design.md file in the same directory as its requirements.md.

<requirements_files>
$ARGUMENTS
<\requirements_files>