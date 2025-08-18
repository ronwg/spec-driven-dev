# Create a Requirements Document

Your task is to transform informal user asks into comprehensive, professional requirements documents following Behavior-Driven Development (BDD) best practices.

## Input

You will receive:
- a free-text user ask describing a feature need, technical requirement, or system behavior.
- (optional) a list of related requirements for integration context 

## Output Format

Generate a requirements.md document with the following structure:

```markdown
# Requirements Document

## Introduction
[2-3 paragraph executive summary that:
- Describes the feature/capability in business terms
- Explains the value proposition and user benefit
- Provides high-level context of how it fits into the system]

## Requirements

### Requirement 1
**User Story:** As a [persona], I want [feature/capability], so that [business value/benefit].

#### Acceptance Criteria
1. WHEN [trigger/condition] THEN the system SHALL [expected behavior]
2. WHEN [another scenario] THEN the system SHALL [another behavior]
3. IF [edge case/error condition] THEN the system SHALL [error handling]
[Continue with 5-8 comprehensive criteria covering happy path, edge cases, and error scenarios]

### Requirement 2
[Continue with additional requirements...]
```

## Transformation Guidelines

### 1. Persona Identification
- Extract all explicit and implicit user personas from the ask
- Consider: end users, administrators, system operators, external systems
- Ensure each persona's needs are represented in at least one requirement

### 2. Requirement Categories to Consider
For each user ask, ensure coverage of:
- **Core Functionality**: Primary feature behavior
- **User Experience**: Interface, feedback, and interaction patterns
- **Edge Cases**: Boundary conditions and unusual scenarios
- **Performance**: Speed, scalability, and resource constraints
- **Error Handling**: Failure scenarios and recovery mechanisms
- **Data Persistence**: Storage, synchronization, and consistency
- **Integration**: Interactions with other system components
- **Security/Privacy**: If applicable to the feature

### 3. Acceptance Criteria Format
- Use WHEN/THEN format for standard scenarios
- Use IF/THEN format for conditional or error scenarios
- Each criterion must be:
  - Testable and measurable
  - Specific and unambiguous
  - Independent (can be tested in isolation)
  - Use "SHALL" for mandatory requirements
  - Include specific values, timeframes, or limits where mentioned

### 4. Technical Details Translation
- Convert technical implementation details into business-readable requirements
- Preserve technical accuracy while ensuring non-technical stakeholders can understand
- Include specific technologies, APIs, or systems mentioned in the user ask
- Add reasonable technical constraints (timeouts, limits, retries) even if not explicitly stated

### 5. Completeness Checklist
Ensure each requirement addresses:
- ✓ Happy path scenarios
- ✓ Error conditions and fallbacks
- ✓ Performance expectations (if applicable)
- ✓ Data handling and persistence (if applicable)
- ✓ User feedback and notifications
- ✓ System state changes
- ✓ Integration points (if applicable)

### 6. Quality Standards
- Use consistent terminology throughout
- Number requirements sequentially
- Write in active voice
- Avoid implementation-specific details unless explicitly required
- Include configurability where flexibility is implied
- Be minimal, create only the necessary requirements – no padding or redundancy  

## Example Patterns

### For UI/UX Features:
- Consider visual feedback, loading states, error messages
- Include accessibility requirements if applicable
- Define interaction patterns and user flows

### For Backend/System Features:
- Include performance metrics and SLAs
- Define data models and persistence requirements
- Specify integration protocols and error handling

### For AI/ML Features:
- Define model selection and parameters
- Include accuracy/confidence thresholds
- Specify fallback behaviors for AI failures

## Special Instructions
1. If the user ask is vague, make reasonable assumptions based on industry best practices
2. If multiple interpretations are possible, choose the most comprehensive one
3. Maintain a professional, formal tone throughout the document
4. Use the exact technical terms and system names mentioned in the user ask

 Create a new directory with the feature/request name, then create a new requirements.md file under this new directory. 
 Transform the provided user ask into a comprehensive BDD requirements document following these guidelines and write them in the newly created requirements.md file. 

<user_ask>
$ARGUMENTS
<\user_ask>
