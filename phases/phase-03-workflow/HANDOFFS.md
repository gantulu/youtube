# Workflow Handoffs

| Handoff | Input | Output |
|---|---|---|
| Input → Analysis | normalized video ID | accessible video evidence |
| Analysis → Reference | evidence + timeline | Global Reference |
| Reference → Scenes | Global Reference + timeline | scene map |
| Scenes → Prompts | scene map + continuity state | prompt plan |
| Prompts → Validation | prompt plan | validation result |
| Validation → Output | passed contracts | structured scene blueprint |

## Principle
Each handoff must carry enough state for the next stage without requiring the next stage to guess missing information.
