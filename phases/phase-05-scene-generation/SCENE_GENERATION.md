# Scene Generation Protocol

## Preconditions
Phase 4 analysis must be complete and its required gate must pass. Generation must use the verified scene map, Global Reference, evidence classifications, and start/end states.

## Scene transformation
For each scene:
1. read the scene evidence;
2. preserve supported characters, objects, environment, visual language, camera, composition, lighting, and audio characteristics;
3. define the intended generated visual state;
4. preserve the scene start/end continuity contract;
5. select the appropriate generation stage.

## Evidence rule
Generation may transform supported evidence into a creative specification, but it must not silently add unsupported source details as if they were observed facts.
