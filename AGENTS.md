# AGENTS.md

## Purpose

This repository is a knowledge base for inclusive, accessible, and evidence-informed VR, XR, and AR design, delivery, and validation. It captures the core principles, methodologies, barriers, techniques, and acceptance tests for teams creating immersive environments and experiences for real users.

This file is intended to optimize agent behavior for:
- project management in VR/XR/AR programs
- design leadership and product strategy
- interaction design and environment design
- engineering implementation and architecture
- QA, accessibility testing, and release readiness
- service, operations, and support planning

Primary source of truth:
- `Inclusive_Design_Guidance_VR_XR_AR.md`

Repository purpose:
- principles, approaches, and methodologies for virtual, augmented, and cross-reality experiences

## Core operating principles for agents

1. Treat accessibility as a product requirement, not an afterthought.
2. Design for comparable value and agency for disabled and non-disabled users.
3. Prioritize user control over exposure, recovery, pacing, and exit.
4. Design the whole journey, not only the in-experience interaction.
5. Make information redundant and interactions substitutable.
6. Separate design assumptions from proven evidence.
7. Capture barriers and tradeoffs explicitly, with owners and tests.
8. Verify performance, comfort, and failure modes in real delivery conditions.
9. Prefer evidence-informed solutions and user testing over assumptions.
10. Keep accessible alternatives operationally valid, not merely nominally available.

## Domain definitions

- XR: umbrella term for immersive and spatial experiences.
- VR: predominantly virtual environments.
- AR: overlays information or objects onto a physical-world view.
- MR: mixed reality, where digital and physical contexts are combined.
- Inclusive XR: experiences that preserve meaningful control over entering, understanding, operating, and leaving the experience.

## Design principles

### 1. Preserve comparable value and agency
- Define the value of the experience first: learning, discovery, social participation, decision-making, challenge, safety, or productivity.
- Do not replace an interactive task with a passive alternative unless the outcome remains comparable.
- Evaluate alternatives against context, effort, privacy, independence, and social equity.

### 2. Remove unnecessary demands before adding settings
- Prefer interactions tolerant of varied reach, precision, speed, and posture.
- Avoid compulsory timed steps, unnecessary two-handed actions, and forced overhead gestures.
- Do not infer preferences from a diagnosis; users may adopt different modes across tasks.

### 3. Make information redundant and interactions substitutable
- Essential meaning must survive through multiple channels: visual, audio, haptic, textual, multimodal.
- Avoid dependence on a single cue like color, a sound, or a vibration.
- Allow users to choose which channels are active without creating overload.

### 4. Let people control exposure and recovery
- Provide pause, help, recentering, settings, and exit before a task becomes demanding.
- Explain changes in immersion, tracking, sound, body representation, and simulated threat.
- Do not promise that virtual content is harmless when it may still affect users physically or emotionally.

### 5. Design the whole journey
- Consider purchase, setup, calibration, use, disruption, recovery, cleaning, updates, and support.
- Record dependency on staff, accessories, mounts, or environmental conditions.

### 6. Treat conflicting needs as design decisions
- Contrast, target size, motion reduction, and caption placement may conflict.
- Resolve tradeoffs explicitly, with documented priorities and user validation.

## Research and design methodology

### Map demands before choosing hardware
- Convert essential tasks into concrete demands: seeing detail, locating sound, remembering instructions, speaking, reaching, balancing, turning, responding quickly, tolerating motion, and maintaining posture.
- Build a capability and context matrix instead of a diagnostic persona list.
- Include combinations such as low vision with limited neck movement or hearing loss with reduced hand sensation.

### Recruit disabled people throughout the lifecycle
- Include disabled users in problem definition, concept evaluation, prototyping, and release review.
- Pay for participation and specialist contributions.
- Cover underrepresented access needs, especially those absent from initial datasets.
- Use accessible recruitment, informed consent, and facilitation practices.

### Prototype physical and digital experience together
- Test fit, mounting, reach, and controls before finalizing the world design.
- Use low-cost prototypes to isolate issues in action, input device, mapping, or environment.
- Make variables easy to change during research: positions, colors, text scale, target tolerance, control mappings, and motion options.

### Separate exploration from validation
- Use facilitated exploration to discover barriers and options.
- Run separate validation tasks with agreed procedures and consistent conditions.
- Record practice effects, carryover, and fatigue.

### Maintain a traceable barrier record
For every observation, capture:
- task
- intended outcome
- device and software version
- settings enabled
- input method
- environment
- access needs
- what happened
- support provided
- root assumption
- proposed change
- owner
- test reference

## Barrier taxonomy

The project organizes barriers into the following categories, with design responses to investigate.

### Motor and physical access
- Controller holding
- Controller orientation
- Input press and hold
- Multiple input complexity
- Reach and balance demands

Example response patterns:
- supported or mounted input
- rest positions
- alternative controllers
- recoverable state transitions
- seated routes and adjusted workspaces
- lowering or bringing objects closer to the user

### Cognitive and comprehension barriers
- Comprehension
- Expectation mismatch
- Wayfinding confusion
- Timing pressure
- Focus and memory load
- Sensory overload or discomfort

Example response patterns:
- consistent affordances and object semantics
- safe practice zones
- on-demand action explanations
- predictable transitions
- persistent objectives and resumable tasks
- adjustable pacing and timeout behavior

### Visual access barriers
- Colour contrast issues
- Determining direction or orientation
- Signage and route discovery
- Small or moving text

Example response patterns:
- configurable contrast and outlines
- stronger landmarks and orientation tools
- accessible destination lists and route queries
- resizable and persistent readable text

## Extended barrier areas

The repo explicitly extends the core barrier list to include:
- absent speech and non-speech audio access
- blind interaction and spatial understanding
- speech recognition failure
- optical fit and binocular differences
- pain and fatigue
- AR-specific conditions such as background visibility, surface detection, anchor drift, camera access, glare, field-of-view limits, and confusion between real and virtual hazards
- shared-space and multiplayer concerns

## Area-specific design guidance

### 1. Physical products and ergonomics
- Evaluate the complete worn configuration: headset, strap, inserts, headphones, cables, battery, tracker.
- Define intended range of head and face dimensions and verify donning, adjustment, removal, and pressure points.
- Test compatibility with spectacles, prescription inserts, hearing aids, and implant components.
- Check posture, duration, and fatigue thresholds.
- Provide safe places to put down devices and support resting arms.

### 2. Input selection and manipulation
- Separate action vocabulary from movement logic: select, confirm, cancel, move, rotate, grab, release, pause, recenter.
- Ensure complete routes for access profiles, including controller, switch, keyboard, touch, voice, head pointing, and gaze.
- Replace sustained or simultaneous actions with toggles, latches, and sequential steps.
- Increase target tolerance while keeping behavior predictable and explicit.
- Treat each input alternative as conditional and provide known fallbacks.

### 3. Movement, orientation, and comfort
- Offer stationary and low-movement routes.
- Provide destination previews and clear arrival orientation cues.
- Distinguish virtual movement from physical movement and avoid misleading physical affordances.
- Reduce motion burden and provide readily available pause and recovery.
- Build orientation into the environment with landmarks and clear spatial relationships.

### 4. Visual and nonvisual access
- Test contrast in context, not in isolation.
- Support resizing, stable placement, and persistence of text.
- Preserve context when magnifying or reducing scale.
- Provide meaningful naming, state, and location for objects.
- Support ordered navigation, object search, and descriptive queries.
- Support nonvisual exploration patterns where appropriate.

### 5. Hearing, speech, and communication
- Preserve essential meaning of sound and dialogue.
- Provide synchronized, usable captions with speaker identification and off-screen information where needed.
- Support sign language, text communication, and alternative participation models.
- Ensure social safety controls are reachable and understandable:
  - mute
  - block
  - report
  - leave
  - distance controls
- Maintain communication continuity when a user pauses, removes the headset, or changes input.

### 6. Cognition, learning, and sensory experience
- Make possibilities and next steps explicit.
- Provide practice spaces and teach actions one at a time.
- Reduce memory and divided-attention demands.
- Offer recovery summaries after interruptions.
- Consider brightness, flashes, repetitive patterns, looming objects, sudden sound, sensorimotor discomfort, and emotional distress.
- Provide calm spaces and accessible modes for low-stimulation operation.

### 7. AR and mixed reality requirements
- Distinguish display mode: optical see-through vs video passthrough vs handheld AR.
- Explain environmental demands before the user starts.
- Account for clutter, reflective surfaces, low-texture surfaces, glare, camera permissions, and field-of-view limits.
- Handle anchors, tracking loss, and occlusion with explicit feedback and recovery paths.
- Preserve attention compatibility with the physical world.
- Make shared AR placement semantics visible and agreed.

### 8. Design redundancies and competing needs
- For every critical message or action, define independent routes and failure modes.
- Test channel loss: audio absent, haptics absent, controller unavailable, degraded tracking.
- Resolve conflicts using explicit priorities and clear user controls.
- Do not remove access features quietly; reduce decorative quality first and preserve essential meaning.

### 9. Software architecture and service design
- Maintain an accessible model of the experience independent of renderer and device input.
- Route input through named actions and update shared state before generating output.
- Persist preferences across sessions and account for updates and guest contexts.
- Provide companion experiences only if they preserve state and support real tasks.
- Explain privacy, security, recording, and operational access in accessible language.
- Include usable support flows for procurement, setup, recovery, support, and venue operations.

### 10. Performance, reliability, and measurement
- Measure real production conditions on supported hardware.
- Evaluate sustained performance, missed frames, latency, tracking stability, and scene motion.
- Preserve access under dynamic resolution, network delay, and recovery events.
- Combine repeatable engineering tests with human evaluation.
- Define measurable targets before release.

## Acceptance test framework

The handbook defines a structured test suite for VR/XR/AR acceptance. Agents should treat these as normative design and QA anchors unless project-specific requirements override them.

### T01 Entry setup and onboarding
- Procedure: start from real booking or installation route and fresh configuration.
- Accept when: the person can discover requirements and complete entry with advertised support; no required accommodation is hidden behind the interaction it replaces.

### T02 Stop, exit, and physical recovery
- Procedure: rehearse stop, pause, quiet-space access, and headset removal before exposure.
- Accept when: the user can initiate stop through an accessible route, stimulation ceases as intended, and physical assistance is available where needed.

### T03 Fit, posture, and sustained comfort
- Procedure: evaluate donning, adjustment, reading, interaction, and removal with the full worn configuration.
- Accept when: tasks do not require painful or unsupported posture; fit remains usable and optical clarity can be maintained.

### T04 Physical handling and recovery
- Procedure: test unpacking, charging, connecting, identifying controls by touch, and recovering a dropped or unreachable device.
- Accept when: each independent action is achievable and any assistance need is declared and workable.

### T05 Complete alternative input routes
- Procedure: run the essential journey with each supported input profile.
- Accept when: all essential actions and feedback remain available without hidden dependence on the default controller, gesture, or speech.

### T06 Targeting precision and confirmation
- Procedure: test small, distant, adjacent, moving, and partly obscured targets.
- Accept when: intentional selection is reliable and consequential actions can be confirmed or corrected.

### T07 Holding, timing, and simultaneous actions
- Procedure: complete grab, drag, teleport, transfer, and timed decisions using alternatives to hold-to-aim or hold-to-grab.
- Accept when: the alternative removes the original sustained or concurrent demand, state is clear, and cancel/release remains available.

### T08 Reach height and balance
- Procedure: repeat tasks seated, standing, and across the intended reach range.
- Accept when: essential content can be accessed without disproportionate posture, reach, or body control requirements.

### T09 Wayfinding and return
- Procedure: navigate to named destinations and return using visual and nonvisual routes.
- Accept when: destination, route, and arrival orientation are clear and wrong turns can be corrected without restart.

### T10 Nonvisual world interaction
- Procedure: locate, identify, select, operate, and verify objects in a blind or nonvisual context.
- Accept when: the user can understand and complete the essential task without inappropriate visual dependency.

### T11 Text contrast and visual discovery
- Procedure: inspect content across backgrounds, lighting, distance, and view positions.
- Accept when: contrast and discovery requirements are met and essential content does not clip, disappear, or require forced posture.

### T12 Captions, audio alternatives, and signing
- Procedure: run content with audio muted and check captions, speaker attribution, and non-speech representations.
- Accept when: essential meaning remains understandable and the presentation does not force inaccessible searching or obscured actions.

### T13 Understanding, memory, and interruption
- Procedure: discover actions, complete a multi-step task, interrupt, and then resume.
- Accept when: the next step and context can be recovered without hidden coaching and tasks remain understandable.

### T14 Sensory settings and transitions
- Procedure: test brightness, sound, movement, and haptics with relevant users under agreed exposure conditions.
- Accept when: optional stimulation can be reduced without losing essential meaning and stop remains accessible.

### T15 Locomotion and motion comfort
- Procedure: compare stationary, teleport, and continuous-movement configurations.
- Accept when: the intended task has a usable lower-motion route and no forced motion remains in essential controls.

### T16 AR visibility and environmental variation
- Procedure: test relevant indoor/outdoor conditions, lighting transitions, clutter, occlusion, and mounted-device use.
- Accept when: essential content remains accessible within the stated envelope and unsupported conditions are identified before misleading guidance is given.

### T17 Tracking loss, anchors, and permission failure
- Procedure: interrupt tracking, obscure a camera, deny permissions, and restore the session.
- Accept when: failure is communicated through usable channels, unintended actions do not occur, and recovery does not require inaccessible remedial actions.

### T18 Settings persistence and combined configurations
- Procedure: combine high-impact settings such as captions, magnification, reduced motion, and switch scanning.
- Accept when: settings remain compatible, persist as intended, and do not remove the recovery route.

### T19 Performance endurance and load
- Procedure: run repeatable production tasks on minimum supported hardware with full access features and realistic load.
- Accept when: performance budgets remain within limits and no inaccessible degradation occurs after extended use or recovery events.

### T20 Social participation and protection
- Procedure: join, communicate, take turns, pause, and rejoin with supported communication modes.
- Accept when: people can contribute to the same meaningful activity without penalties based on access method.

### T21 Channel loss and redundancy
- Procedure: remove one output or input dependency at a time and test remaining routes.
- Accept when: the remaining route conveys enough meaning to act or safely stop the task.

### T22 Privacy, assistance, and companion control
- Procedure: review consent, recording, preference visibility, and companion-device failure.
- Accept when: people can make informed choices and distinguish their actions from a helper's without data exposure or task strand.

### T23 Service delivery and support
- Procedure: rehearse booking, arrival, fitting, stop event, equipment fault, debrief, cleaning, and next-user preparation.
- Accept when: staff can provide the stated support consistently and users can obtain help without inaccessible barriers.

### T24 Comparable outcomes across modes
- Procedure: compare headset, adapted, and non-headset routes against the same purpose.
- Accept when: alternatives preserve the essential outcome and agency or any remaining difference is transparently justified.

## Release and governance gates

Do not release a VR/XR/AR product or environment when any of the following remain unresolved:
- inability to stop or recover safely
- misleading safety-critical information
- severe failure in an advertised essential route
- unsupported high-risk barriers in user-critical tasks
- inability to communicate or give clear user agency

Release decisions should include evidence from:
- user testing
- failure-mode analysis
- performance and reliability evidence
- service and staffing readiness
- support and fallback procedures
- version-specific regression review

## Agent decision rules

When planning or reviewing a VR/XR/AR project, agents should:
- map essential tasks to demanded capabilities
- identify the access ecosystem: hardware, software, environment, support staff, companion devices
- verify whether the system preserves agency, recovery, and comparable outcomes
- check whether alternatives are independent of the same hidden dependency
- prefer explicit user control over silent adaptation
- record unresolved barriers with ownership and mitigation status
- test both nominal behavior and degraded conditions

## Preferred output patterns for agents

When generating recommendations, project plans, or reports, prefer:
- task-based requirement statements
- access-demand matrices
- barrier records with owner and remediation status
- test references tied to the acceptance suite
- measured outcomes and failure conditions
- clear statement of what remains unsupported and why

## Repository-specific guidance

Treat this repository as a design and QA framework for immersive experiences, not merely a general accessibility checklist.

Priority concerns:
- mobility and posture
- sensory load and comfort
- visual and nonvisual access
- hearing and communication
- cognition and memory
- safety and stop/recovery
- social participation and fairness
- performance under real conditions
- service delivery and environment readiness

## References inside the repo

The handbook and project data reference:
- BBC barriers research
- W3C XR Accessibility User Requirements
- TetraLogical XR accessibility guidance
- Apple and Meta platform accessibility guidance
- WCAG 2.2 where relevant to interface contrast and presentation
- supplementary research on motion sickness, visual accommodation conflicts, haptic/auditory nonvisual interaction, and low-vision support

## Minimal agent instruction summary

If you are an agent working in this repository, operate as follows:

- start from user need and task outcome
- map access demands before implementation
- design redundant and substitutable pathways
- ensure stop, pause, recovery, and safe exit are always available
- test under real conditions and degraded conditions
- document barriers, owners, and acceptance criteria
- do not assume one sensory channel or one control path is sufficient
- preserve agency, comfort, and comparable value across access profiles
- validate the full experience journey, not just the core interaction

## Citation source note

The strategic content in this file is drawn from the repository's inclusive XR handbook and should be treated as a practical operational summary for agents and design teams working on immersive, spatial, and mixed reality projects.

This file is optimized for LLM and agent consumption: concise enough for instruction-following, rich enough to capture methodologies, barriers, patterns, and testing logic, and structured for use across design, engineering, QA, and project governance.
