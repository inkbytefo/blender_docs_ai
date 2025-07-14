---
type: "always_apply"
---

# Prompt Engineering Guidelines for Blender AI Agent

## Overview
This document outlines the prompt engineering best practices specifically tailored for the Blender AI Agent that operates through Blender MCP and ScreenMonitorMCP integration. These guidelines ensure optimal performance, clear communication, and effective 3D content creation workflows.

## Core Prompt Engineering Principles

### 1. Clarity and Specificity
- **Be Explicit**: Clearly state what you want to achieve
- **Avoid Ambiguity**: Use precise terminology and specific measurements
- **Provide Context**: Explain the purpose and intended use of the 3D content
- **Set Expectations**: Define quality levels, timelines, and constraints

#### Examples of Clear Prompts
```
❌ Poor: "Make a car"
✅ Good: "Create a realistic sports car model with detailed exterior, focusing on aerodynamic design, using metallic paint materials, suitable for product visualization rendering"

❌ Poor: "Fix the lighting"
✅ Good: "Analyze the current lighting setup and improve it for product photography, ensuring even illumination with minimal harsh shadows, using a three-point lighting configuration"
```

### 2. Structured Request Format
Use a consistent format for complex requests to ensure all necessary information is provided:

```
**Objective**: [What you want to create/modify]
**Context**: [Purpose, style, or use case]
**Requirements**: [Specific constraints or specifications]
**Quality**: [Draft, production, photorealistic, etc.]
**Validation**: [How success should be measured]
```

#### Example Structured Request
```
**Objective**: Create a championship trophy
**Context**: Award ceremony for a technology competition
**Requirements**: Modern design, 30cm height, metallic finish, company logo placement
**Quality**: Photorealistic for marketing materials
**Validation**: Must look professional in rendered images
```

### 3. Progressive Complexity
Start simple and add complexity gradually:

#### Phase 1: Basic Structure
"Create the basic shape and proportions"

#### Phase 2: Detail Addition
"Add surface details and refinements"

#### Phase 3: Material Application
"Apply realistic materials and textures"

#### Phase 4: Lighting and Rendering
"Set up lighting and prepare for final rendering"

### 4. Feedback Integration Patterns

#### Iterative Feedback
- "Show me the current progress and let me provide feedback"
- "Create this step-by-step, pausing for validation at each stage"
- "Let me review the basic shape before adding details"

#### Specific Feedback
- "The proportions look good, but make the base 20% wider"
- "The material is too reflective, reduce the metallic value to 0.3"
- "The lighting creates too much contrast, soften the shadows"

## Tool-Specific Prompt Patterns

### 1. Blender MCP Operations

#### Scene Setup Prompts
```
"Initialize a clean scene with proper lighting for [project type]"
"Set up the workspace with [specific viewport configuration]"
"Prepare the scene for [modeling/animation/rendering] workflow"
```

#### Modeling Prompts
```
"Create a [object] using [specific technique] with [quality level] detail"
"Model a [object] following [industry standard/style] guidelines"
"Generate [object] with proper topology for [intended use]"
```

#### Material Prompts
```
"Create a [material type] material with [specific properties]"
"Set up a procedural [texture type] using shader nodes"
"Apply PBR materials suitable for [rendering engine]"
```

### 2. ScreenMonitorMCP Analysis

#### Visual Validation Prompts
```
"Analyze the current scene and verify [specific aspect]"
"Check if the [object/material/lighting] meets [quality standard]"
"Compare the current result with [reference/expectation]"
```

#### Progress Monitoring
```
"Monitor the modeling progress and alert if issues arise"
"Track the visual changes during [specific operation]"
"Validate each step of the [workflow type] process"
```

## Advanced Prompt Engineering Techniques

### 1. Chain-of-Thought Prompting
Break complex tasks into logical steps:

```
"To create a realistic donut:
1. First, analyze the basic geometry requirements
2. Create the torus shape with proper proportions
3. Add surface imperfections for realism
4. Apply procedural materials for the dough and icing
5. Set up appropriate lighting for food photography
6. Validate each step visually before proceeding"
```

### 2. Few-Shot Learning
Provide examples of successful patterns:

```
"Similar to how we created the previous trophy:
- Start with basic geometric shapes
- Use boolean operations for complex forms
- Apply metallic materials with proper reflectance
- Set up studio lighting for product shots
Now create a medal following the same approach"
```

### 3. Role-Based Prompting
Define specific expertise contexts:

```
"Acting as a professional 3D artist specializing in architectural visualization:
Create a modern office building exterior with attention to:
- Realistic proportions and scale
- Appropriate material choices
- Professional lighting setup
- Industry-standard modeling techniques"
```

### 4. Constraint-Based Prompting
Clearly define limitations and requirements:

```
"Create a character model with these constraints:
- Maximum 10,000 polygons for game optimization
- Clean quad topology for animation
- UV mapped for 2K texture resolution
- Rigging-friendly edge flow
- Validation through wireframe analysis"
```

## Error Prevention and Recovery

### 1. Anticipatory Prompting
Include potential issues in your prompts:

```
"Create a complex mechanical assembly, ensuring:
- No overlapping geometry
- Proper scale relationships
- Manageable polygon count
- Clear component separation
- Performance optimization for real-time preview"
```

### 2. Validation Checkpoints
Build in verification steps:

```
"After each major operation:
1. Capture a screenshot for visual verification
2. Check for geometric errors or artifacts
3. Validate against the original requirements
4. Confirm before proceeding to the next step"
```

### 3. Recovery Procedures
Define fallback strategies:

```
"If the current approach isn't working:
1. Analyze what went wrong using visual feedback
2. Suggest alternative methods
3. Implement the most promising approach
4. Document the successful solution for future reference"
```

## Quality Assurance Prompts

### 1. Technical Validation
```
"Verify that the model meets technical specifications:
- Proper scale and proportions
- Clean topology without errors
- Appropriate polygon density
- Correct normal directions
- Suitable UV mapping"
```

### 2. Visual Quality Assessment
```
"Evaluate the visual quality:
- Realistic material appearance
- Appropriate lighting and shadows
- Proper color balance and contrast
- Professional composition and framing
- Absence of visual artifacts"
```

### 3. Performance Validation
```
"Check performance characteristics:
- Acceptable polygon count for intended use
- Optimized texture memory usage
- Efficient material setup
- Reasonable render times
- Stable viewport performance"
```

## Communication Optimization

### 1. Progress Reporting Requests
```
"Provide regular updates on:
- Current operation status
- Visual validation results
- Any issues encountered
- Estimated completion time
- Next steps in the workflow"
```

### 2. Learning Integration
```
"Document this workflow for future reference:
- Record successful operation sequences
- Note any optimization opportunities
- Capture visual results for comparison
- Create reusable templates
- Build knowledge base entries"
```

### 3. Collaborative Feedback
```
"Explain your approach so I can:
- Understand the technical decisions
- Provide informed feedback
- Learn from the process
- Suggest improvements
- Collaborate more effectively"
```

## Best Practices Summary

### Do's
- ✅ Be specific and detailed in requests
- ✅ Provide clear context and purpose
- ✅ Use structured request formats
- ✅ Build in validation checkpoints
- ✅ Request explanations for learning
- ✅ Document successful workflows
- ✅ Provide specific feedback
- ✅ Use progressive complexity

### Don'ts
- ❌ Use vague or ambiguous language
- ❌ Skip context or purpose information
- ❌ Rush through complex operations
- ❌ Ignore visual validation steps
- ❌ Forget to specify quality requirements
- ❌ Overlook performance considerations
- ❌ Skip documentation of success patterns
- ❌ Provide non-specific feedback

## Continuous Improvement

### Feedback Loop Optimization
- Regularly review and refine prompt patterns
- Learn from successful and unsuccessful interactions
- Adapt prompts based on agent capabilities
- Incorporate new techniques and best practices
- Share effective patterns with the community

### Pattern Recognition
- Identify successful prompt structures
- Document effective communication patterns
- Build libraries of proven approaches
- Create templates for common scenarios
- Develop expertise in specific domains

### Innovation and Experimentation
- Test new prompt engineering techniques
- Explore advanced interaction patterns
- Experiment with different communication styles
- Integrate emerging best practices
- Contribute to the evolution of AI-human collaboration
