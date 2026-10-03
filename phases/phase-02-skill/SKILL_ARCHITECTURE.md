# Gemini Skill Architecture

## Layers
1. Identity — expert YouTube Shorts Video Understanding AI Agent, Video Analyst, Scene Decomposer, Prompt Engineer.
2. Input contract — URL or video ID normalization.
3. Evidence policy — actual video is primary evidence; metadata alone is insufficient.
4. Analysis workflow — complete timeline, visual + audio, timestamps, rapid-event verification.
5. Reference model — global reference plus persistent character/object/environment identity.
6. Generation planning — scene anchor, image-to-image continuity, image-to-video, extension.
7. Validation — structural, temporal, prompt, continuity, and audio checks.
8. Output contract — scene blueprint only after gates pass.

## Separation of concerns
Knowledge answers what is true/supported. Skill answers how Gemini should operate. Later workflow artifacts answer how the system is executed. Validator artifacts answer how output is checked.

## Non-goals
The Skill must not claim unsupported model capabilities, invent evidence, or replace current official documentation for volatile model information.
