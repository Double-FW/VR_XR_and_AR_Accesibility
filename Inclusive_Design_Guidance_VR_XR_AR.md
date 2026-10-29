# Inclusive design guidance for VR, XR and Augmented Reality

## Practical guidance for physical products digital experiences and services

28 October 2026

Inclusive XR gives people meaningful control over how they enter, understand, operate and leave an experience. Success depends on the combined design of the device, its physical environment, the software and the service around it. An accessible menu cannot compensate for a headset someone cannot wear; a comfortable headset cannot compensate for an interaction they cannot perform.

This handbook is for product owners, industrial designers, interaction designers, content teams, engineers, researchers, procurement teams and operators. It translates observed barriers and supporting research into design decisions, alternative approaches and tests. It covers head-mounted VR, 360-degree media, mixed reality, optical and video passthrough AR, and handheld AR. The recommended outcome is a comparable experience with agency, dignity, comfort and useful participation, rather than a checklist pass alone.

## How to use this handbook

Begin with the principles and evidence boundaries in Chapters 1 and 2. Use Chapter 4 as the barrier index, Chapters 5 to 13 during design and implementation, and Chapters 14 to 16 to plan verification and release. Chapter 17 shows how the recommendations work together in one experience. Sources are collected in Chapter 18; bracketed source identifiers link to those entries. Test identifiers refer to Chapter 15.

Recommendations and acceptance criteria are this handbook's synthesis unless explicitly described as a source finding or a standard requirement. They are intended to be adopted and refined for a defined product and audience. They are not claims that every technique has been experimentally validated, nor universal medical or ergonomic limits.

## Contents

Select a chapter or use Word's Navigation Pane. Source identifiers and test numbers throughout the handbook are also linked.

[1 Evidence and scope](#1-evidence-and-scope)

[2 Design principles](#2-design-principles)

[3 Research and design methodology](#3-research-and-design-methodology)

[4 Catalogue of identified barriers](#4-catalogue-of-identified-barriers)

[5 Physical products and ergonomics](#5-physical-products-and-ergonomics)

[6 Input selection and manipulation](#6-input-selection-and-manipulation)

[7 Movement orientation and comfort](#7-movement-orientation-and-comfort)

[8 Visual and nonvisual access](#8-visual-and-nonvisual-access)

[9 Hearing speech and communication](#9-hearing-speech-and-communication)

[10 Cognition learning and sensory experience](#10-cognition-learning-and-sensory-experience)

[11 Additional requirements for AR and mixed reality](#11-additional-requirements-for-ar-and-mixed-reality)

[12 Design redundancies and competing needs](#12-design-redundancies-and-competing-needs)

[13 Software architecture and service design](#13-software-architecture-and-service-design)

[14 Performance reliability and measurement](#14-performance-reliability-and-measurement)

[15 Test programme and acceptance criteria](#15-test-programme-and-acceptance-criteria)

[16 Safe sessions release and ongoing improvement](#16-safe-sessions-release-and-ongoing-improvement)

[17 Worked example of an inclusive experience](#17-worked-example-of-an-inclusive-experience)

[18 Sources and evidence notes](#18-sources-and-evidence-notes)

# 1 Evidence and scope

## Working definitions

XR is used here as an umbrella for immersive and spatial experiences. VR presents a predominantly virtual environment; AR adds information or objects to a view of the physical world; MR commonly describes experiences that align and interact with physical surroundings. Product labels vary, so requirements should identify the actual display, tracking and interaction behaviour. A 360-degree video normally lets the viewer look around recorded content but does not offer the positional exploration of a fully modelled scene. Test these formats separately rather than treating all headset content as equivalent.

## What the research establishes

The BBC Barriers Browser describes approximately 1,700 observations involving over 100 research participants. Its strongest contribution is a taxonomy of ways that immersive environments assume particular bodies, senses, knowledge and movement. The work concentrated on VR and 360-degree video. It reports that similar barriers occur in AR and MR, but does not provide equivalent AR evaluation detail. Applying its findings to AR therefore requires additional contextual validation. \[B01\]

The project was interrupted by COVID-19. Barriers Browser explicitly reports insufficient data from blind, Deaf and hard-of-hearing users for their inclusion in the analysis. Its counts are observations, not prevalence estimates; repeated observations are not independent participants. The presentations describe evolving stages of the research, so their interim participant and barrier counts should not be combined as a single statistical dataset. \[B01, B02, B03, B12\]

There are 15 named barrier categories in the supplied browser: five motor, six cognitive and four low-vision categories. Its introductory total of 14 is inconsistent with that list. This handbook retains all 15 and preserves the original category numbers, without treating the stated total as authoritative. The categories overlap and are not diagnostic profiles. \[B01\]

## Distinguish findings from proposed responses

The BBC switch and low-vision documents describe adaptations developed to remove large barriers so smaller ones could be observed. They explicitly avoid presenting these as general recommended solutions. They offer valuable design hypotheses and local findings, not universal effectiveness claims. \[B04, B05\]

For example, the low-vision report says high-contrast hands helped its participants and that distinctive views improved orientation within the main room. It also records unresolved signage difficulties. The report mentions ten participants in its introduction but six in several findings, and contains unfinished and duplicated material. Do not convert those statements into population success rates. The practical implication is to test configurable contrast and orientation cues, while retaining alternatives to signage. \[B05, pp 2, 5, 9, 12–13\]

Use the following distinctions when recording evidence. A recommendation can be useful without being a proven universal rule, but its status must remain visible.

| **Evidence type**                  | **What it supports**                                                   | **What it does not establish**                           |
| ---------------------------------- | ---------------------------------------------------------------------- | -------------------------------------------------------- |
| Observed barrier                   | A documented way an interaction excluded or burdened someone           | How common the barrier is across all XR users            |
| Evaluated adaptation or experiment | A technique worth considering under the reported conditions            | Effectiveness across devices, populations and activities |
| Standards or expert guidance       | A structured account of needs, design practices or applicable criteria | Proof that a specific implementation is usable           |
| Platform documentation             | Available features and implementation expectations for that platform   | Equivalent behaviour on other products or versions       |
| Handbook synthesis                 | A proposed design or test response to the evidence                     | A completed validation study or certification            |

## Compliance as one input

W3C's XR Accessibility User Requirements is a Working Group Note, not a conformance standard or a set of baseline requirements. Its coverage includes alternative input and output, personalisation, semantics, orientation, timing and access to recovery controls. Use it to review completeness and allocate responsibilities between application and platform. \[W01\]

TetraLogical's introduction brings these XR requirements together with the BBC barriers and stresses evaluation with disabled people. That combination is a useful basis for practice: standards organise questions, observed barriers challenge assumptions, and product research tests the proposed response. \[W02\]

WCAG 2.2 provides testable criteria for web content and is relevant to web-based menus, account flows and companion services. Its principles can inform spatial interfaces, but a WCAG result does not establish headset fit, physical safety, tolerable motion or access to a three-dimensional task. Its own scope acknowledges that it does not address every user need. \[W16\]

Meta's linked 2020 announcement described the new accessibility VRCs as recommendations at that time. Treat that article as historical context, not evidence of today's store requirements. Apple documents accessibility features available during setup and subsequent use, including VoiceOver, Zoom and Switch Control; their availability does not prove that a custom app exposes usable content to them. \[W03, W04\]

## Scope of confidence

This is an evidence-informed practice handbook, not a systematic review, product certification or clinical protocol. Much of the supplied evidence concerns specific older hardware and small exploratory sessions. Stronger confidence comes from several forms of evidence agreeing, followed by successful testing of the actual product with the intended users. Keep uncertainty explicit for outdoor AR, prolonged occupational use, unusual body positions, combined sensory impairments, children and safety-critical applications.

# 2 Design principles

## Preserve comparable value and agency

The Inclusive Design Principles call for comparable experience, attention to context, consistency, control, choice, prioritisation and added value. Applied to XR, they support preserving the purpose and quality of the experience while allowing different ways to participate. \[W17\]

Define the value first. In a museum, it may be discovering and interpreting an object; in training, it may be making the correct decision; in a game, it may include challenge, exploration and social participation. Physical imitation is not automatically essential. A person can learn about an artefact without walking around it, and can select a virtual tool without gripping a replica.

Assess alternatives against content, available decisions, feedback, privacy, independence, effort and social standing. A passive video is not a comparable replacement for an interactive decision-making task. A non-headset version may be a valuable route, but should preserve the relevant learning, creativity or participation, rather than function as an inferior holding area.

## Remove unnecessary demands before adding settings

Start with interactions that tolerate varied reach, precision, speed and posture. Remove gratuitous timed steps, compulsory two-handed actions and repeated overhead gestures. Then offer personalisation for differences that cannot be resolved through a single design. A long settings menu is not a substitute for a usable default.

Do not infer preferences from a diagnosis. Someone may use direct touch for one action, switch input for another and speech when tired. Needs may change during a session. The BBC switch work found no single best scheme and described changes driven by fatigue, activity and learning. \[B04, p 8\]

## Make information redundant and interactions substitutable

Communicate essential meaning through usable alternatives. A warning should not depend solely on colour, a sound, a vibration or an object outside the current view. Alternative input must reach the same underlying action and outcome. Two controls are not independent alternatives if both require precise pointing or sustained head movement.

Allow people to choose which channels operate. Simultaneous narration, captions, flashing outlines and vibration can increase overload. The goal is recoverable access to meaning, not maximum stimulation. Chapter 12 defines a method for testing whether redundancy is real.

## Let people control exposure and recovery

Make pause, help, recentering, settings and exit available before the experience becomes demanding. Separate a quiet virtual space from returning awareness of the physical environment and from physically removing the device. These are different actions and may need different controls or assistance.

Explain changes in immersion, movement, sound, body representation and simulated threat before they happen. Do not promise that virtual content cannot affect someone physically or emotionally. Agree how support will be offered and how the participant will signal stop. \[B02, B06, B10\]

## Design the whole journey

Include discovery, purchase or booking, transport and arrival, unboxing, charging, setup, identity checks, calibration, use, recovery, cleaning, updates and support. Record where access depends on another person. Assistance can be a chosen and useful part of an experience; it should not be an undisclosed prerequisite for an otherwise advertised independent task.

## Treat conflicting needs as design decisions

Higher contrast may increase glare; a larger target may obscure another target; a stabilised pointer may introduce lag; a persistent caption may cover an important object. Avoid declaring one option universally accessible. Expose meaningful controls, preserve a clear reset route and test combinations. Changes that improve one measure must be checked for new barriers elsewhere.

# 3 Research and design methodology

## Map demands and exclusion before choosing hardware

Describe each essential task in terms of what it demands: seeing detail, locating sound, remembering instructions, speaking, holding, reaching, turning, balancing, responding quickly or tolerating contact and motion. Map those demands onto the device, app and physical setting. Include steps that are easy to overlook, such as retrieving a dropped controller, entering a pairing code and finding the exit after tracking fails.

Build a capability and context matrix rather than a list of diagnostic personas. Include combinations such as low vision with limited neck movement, hearing loss with reduced hand sensation, or a wheelchair user with one hand occupied. Include temporary injury, fluctuating fatigue, an unfamiliar language, noisy surroundings and a mounted phone. Mark requirements that the proposed hardware cannot meet before committing to it.

## Recruit and work with disabled people throughout

Invite disabled people into problem definition, concept evaluation, prototyping and release review. Pay for participation and specialist contributions. Offer accessible recruitment, consent and feedback formats, communication support, travel arrangements and familiar support people where wanted. Include people who have not previously used XR; successful users of an existing platform are not the entire potential audience.

Recruit deliberately to cover underrepresented access needs, especially those absent from the BBC dataset. Include blind participants, Deaf sign-language users, hard-of-hearing participants, people with speech differences, and people with combined impairments. For children or people who need supported consent, establish an appropriate ethics and safeguarding process rather than simply copying an adult session plan.

The BBC quickstart guide demonstrates that location affects who can participate and describes taking a portable lab into different settings. Apply that lesson to recruitment, while reassessing the suitability of every venue and device. Its example room dimensions and lighting arrangements are historical setup details, not universal safe-space specifications. \[B06\]

## Prototype the physical and digital experience together

Test fit, mounting, reach and controls before committing to a visually elaborate world. Use low-cost prototypes to isolate whether a failure concerns the action, the input device, the mapping or the explanation. Follow with an integrated prototype: a control that works on a desk may fail when the headset blocks the user's view or when the armrests occlude tracking.

Make important variables easy to change during research: object positions, colours, text scale, target tolerance, control mappings, motion options and assistance levels. The BBC low-vision work demonstrates the value of an environment that could be changed quickly between observations. Keep configuration changes logged so results remain interpretable. \[B05, p 6\]

## Separate exploration from validation

Use facilitated exploration to discover barriers and develop options. Allow explanation and adaptation, but record exactly when they were needed. Then run a distinct validation task with the agreed onboarding and support model. A task completed after an unplanned facilitator intervention is not evidence of independent success.

For comparisons, keep the objective and content stable, provide comparable familiarisation, and counterbalance order where feasible. Record carry-over from practice and fatigue. Do not repeatedly expose a participant to an inaccessible or uncomfortable condition merely to complete a balanced dataset.

## Build a traceable barrier record

For every observation, capture the task, intended outcome, device and software version, enabled settings, input method, environment, relevant access needs, what happened, support provided and the participant's account. Describe observable behaviour separately from interpretation. "The target was missed four times after the arm became tired" is more useful than "poor motor ability".

Deduplicate related observations without discarding context. Link each barrier to the design assumption, a proposed change, an owner and a test. Preserve contradictory findings. A common workaround may reveal a missing feature; a rare inability to stop may deserve higher priority than a frequent cosmetic inconvenience. The BBC observation-to-barrier pipeline provides the methodological starting point. \[B02, B03\]

# 4 Catalogue of identified barriers

The following catalogue paraphrases all 15 named BBC categories. The responses are proposed design directions, not a claim that the BBC proved them effective. Read the category across impairments and contexts. A visual target can create both a seeing barrier and an aiming barrier; a timed instruction can combine reading, memory and movement demands. \[B01\]

| **BBC category**           | **Demand that creates the barrier**                                               | **Response to investigate and linked tests**                                                                                                                                                                                       |
| -------------------------- | --------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1.1 Controller holding     | Sustaining a grip, location or orientation; recovering a dropped device           | Supported or mounted input, rest positions, alternative controls and recoverable objects. [T03](#t03-fit-posture-and-sustained-comfort), [T04](#t04-physical-handling-and-recovery), [T05](#t05-complete-alternative-input-routes) |
| 1.2 Controller orientation | Repeated accurate aiming or rotation, including while targets move                | Adjustable tolerance, selection lists, axis constraints and independent confirmation. [T05](#t05-complete-alternative-input-routes), [T06](#t06-targeting-precision-and-confirmation)                                              |
| 1.3 Input press and hold   | Maintaining pressure, especially while moving                                     | Toggle, latch or sequential activation, with clear state and cancellation. [T05](#t05-complete-alternative-input-routes), [T07](#t07-holding-timing-and-simultaneous-actions)                                                      |
| 1.4 Multiple input         | Simultaneous buttons, multiple controllers or coordinated movements               | Single-device routes, sequential actions and assisted manipulation. [T05](#t05-complete-alternative-input-routes), [T07](#t07-holding-timing-and-simultaneous-actions)                                                             |
| 1.5 Reach and balance      | Reaching overhead or to the floor, leaning or maintaining balance                 | Bring objects to the person, seated routes, adjustable workspace and retrieval. [T03](#t03-fit-posture-and-sustained-comfort), [T08](#t08-reach-height-and-balance)                                                                |
| 2.1 Comprehension          | Inferring what is possible, interactive or next                                   | Consistent affordances, a safe practice area and on-demand action explanations. [T01](#t01-entry-setup-and-onboarding), [T13](#t13-understanding-memory-and-interruption)                                                          |
| 2.2 Expectation            | Unexpected feedback, body representation or a threatening situation               | Preview transitions, predictable responses and meaningful control over exposure. [T02](#t02-stop-exit-and-physical-recovery), [T13](#t13-understanding-memory-and-interruption), [T14](#t14-sensory-settings-and-transitions)      |
| 2.3 Way finding            | Discovering a route or achieving precise positioning                              | Named destinations, landmarks, guidance and forgiving arrival zones. [T09](#t09-way-finding-and-return), [T10](#t10-nonvisual-world-interaction)                                                                                   |
| 2.4 Timing                 | Acting before an interaction, narrative or decision expires                       | Adjustable pacing, pause, replay and equivalent untimed routes. [T07](#t07-holding-timing-and-simultaneous-actions), [T13](#t13-understanding-memory-and-interruption)                                                             |
| 2.5 Focus and memory       | Remembering controls and goals, maintaining focus or recovering after distraction | Persistent objectives, consistent mappings, resumable tasks and selective prompts. [T13](#t13-understanding-memory-and-interruption), [T18](#t18-settings-persistence-and-combined-configurations)                                 |
| 2.6 Sensory                | Intolerable physical contact, sound, brightness, texture or movement              | Fit options, adjustable sensory content and easy reduction of stimulation. [T03](#t03-fit-posture-and-sustained-comfort), [T14](#t14-sensory-settings-and-transitions), [T15](#t15-locomotion-and-motion-comfort)                  |
| 3.1 Colour contrast        | Separating hands, objects or scene features from changing backgrounds             | Configurable contrast, outlines or backplates, tested across the scene. [T11](#t11-text-contrast-and-visual-discovery)                                                                                                             |
| 3.2 Determining direction  | Identifying orientation, including in symmetric environments or after movement    | Distinctive landmarks, orientation queries and stable arrival conventions. [T09](#t09-way-finding-and-return), [T10](#t10-nonvisual-world-interaction)                                                                             |
| 3.3 Signage                | Discovering and reading signs from the available position and direction           | Multi-directional signs, accessible copies and alternatives to visual routing. [T09](#t09-way-finding-and-return), [T11](#t11-text-contrast-and-visual-discovery)                                                                  |
| 3.4 Text                   | Reading small, moving or short-lived information                                  | Resizable stationary presentation, persistence, replay and read-aloud. [T11](#t11-text-contrast-and-visual-discovery), [T12](#t12-captions-audio-alternatives-and-signing)                                                         |

## Extend the catalogue beyond the original sample

Add explicit records for absent speech and non-speech audio access; blind interaction and spatial understanding; speech recognition failure; optical fit and binocular differences; pain and fatigue; motion intolerance; headset removal; privacy; inaccessible communication and moderation; and installation, authentication and support. These are extensions of scope, not newly discovered BBC categories.

For AR, also record background visibility, surface detection, anchor drift, camera access, glare, tracking conditions, field-of-view limits and confusion between real and virtual hazards. For shared XR, record interpersonal distance, consent to assistance, social pressure to continue and exclusion caused by communication latency. Chapters 5 to 13 develop these additional considerations.

# 5 Physical products and ergonomics

## Headset mass balance and fit

Evaluate the complete worn configuration, including straps, optical inserts, headphones, cables, batteries and any attached tracker. In an experiment with 20 young adults, headset mass and its distance from the head affected estimated cervical torques. Counterweights reduced some upper-neck torques but did not reduce lower-neck torques in the same way. This supports considering mass distribution and movement together; it does not establish a safe weight or validate improvised counterweights for disabled users. \[E01\]

Specify the intended range of head and face dimensions, adjustment travel, contact areas and compatible accessories. Test putting on, adjusting and removing the product, not just wearing it after a researcher has fitted it. Include varied hair, head coverings, facial anatomy and skin sensitivity. Offer options without assuming that a tighter strap is the answer to slipping.

Check pressure around the forehead, cheeks, nose, temples and back of the head, and whether fit changes during speech or head movement. Observe both local pressure discomfort and neck effort. Assess heat, sweat, lens fogging, ventilation noise and cleaning materials in the intended conditions. Do not block vents, sensors or release mechanisms with an adaptation.

Apple's guidance illustrates the interaction between optical alignment, fit and comfort: the suitable light seal, vision correction and eye-to-display alignment matter, and some users fall outside the device's supported interpupillary range. These are product-specific constraints. Procurement should verify the actual accommodation range and supported prescription options rather than assuming "adjustable" means suitable for everyone. \[W12\]

## Vision correction and sensory compatibility

Check whether a device supports spectacles, prescription inserts or contact lenses, and explain this before booking or purchase. Test compatibility with hearing aids, cochlear implant components and other worn equipment according to the relevant manufacturers' guidance. Do not ask someone to remove essential equipment merely to make the demo fit.

A clear image in the centre of the lenses does not prove comfortable viewing across the task. Test text, objects and controls at the actual viewing positions with the person's usual correction. Provide alternatives to stereoscopic depth cues and binocular selection. Record calibration failures as product barriers rather than participant errors.

## Handheld devices and controllers

Evaluate mass, centre of gravity, grip shape, surface texture, trigger force and travel, button separation and discoverability by touch. Include small and large hands, left- and right-handed use, limited finger isolation, involuntary movement and reduced sensation. A nominally light controller can still be difficult to hold at arm's length.

Allow supported arms and resting hands. Avoid requiring controllers to remain visible in the headset merely to maintain an object or menu state. Provide a safe place to put down devices and an accessible way to resume. Straps may help retain a controller but can create fitting, release and sensory barriers; test them as part of the interaction rather than treating them as a complete solution. \[B01, B03, B04\]

For phones and tablets, support one-handed use, mounted use and landscape or portrait arrangements where appropriate. Avoid sustained camera aiming while operating small controls with the same hand. Offer a frozen inspection view, model viewer or remote control route when live camera movement is not essential. Check that these modes retain the information needed for the task.

## Mounts switches and mobility equipment

Select switch type, activation force, size and position with the person. Verify that mounting does not interfere with wheelchair controls, transfers, brakes, communication devices or pressure relief. Protect cables from wheels and moving joints. Use secure, appropriate mounting systems and a planned release route; do not generalise the BBC's prototype zip-tie arrangements into a production installation method. \[B04\]

Head-controlled pointing transfers work from the hand to the neck. Chair-controlled pointing transfers work to manoeuvring and clearance. Test that transfer of demand explicitly. Prefer software use of available tracking over adding mass to a headset, where feasible. An adaptation should not create a new physical burden that is hidden by a successful task score.

## Workspace posture and duration

Let people define a comfortable working zone while seated, standing or using their normal support. Put frequent interactions near that zone and bring infrequent objects into it. Avoid inferring reach from height alone. Accommodate armrests, trays, headrests and a reclined posture when the product supports it. Recheck virtual height and orientation after posture changes.

Evaluate short use, repeated tasks and intended session duration. Record when discomfort or fatigue begins, where it occurs and which action preceded it. A successful first minute does not establish tolerable sustained use. Breaks must be possible without losing progress, credentials, position in a queue or access to collaborators.

Use device-specific safety and break guidance as a starting point, with earlier stops whenever needed. Apple advises stopping when discomfort occurs rather than waiting for a scheduled break. No duration in this handbook is a guaranteed safe exposure for every person. \[W11\]

# 6 Input selection and manipulation

## Separate the action from the movement

Define an action vocabulary such as select, confirm, cancel, move, rotate, grab, release, pause and recenter. Map each action to supported inputs, rather than writing application logic that only responds to a particular hand pose. Keep feedback, permissions and results consistent across mappings.

Provide complete routes for the intended access profiles. Depending on the platform and task, these may include one controller, switches with scanning, keyboard, touch, voice, head pointing or gaze. Do not advertise support because an input can open a menu while the main activity still requires two hands. A user's chosen input must also reach settings, help and exit.

The BBC experiments distinguish hardware selection and placement from software mapping. This is essential: connecting a switch does not make a spatial interface switch accessible. The software may still require a cursor, aim, release timing or physical rotation that the person cannot supply. \[B04, B06\]

## Replace sustained and simultaneous actions

Offer press-on and press-off alternatives to hold-to-grab or hold-to-aim, with an unambiguous latched state. Make release, cancel and emergency stop separately discoverable. Avoid a hidden timeout that drops an object when the user pauses. For deliberate dragging or manipulation, provide stepwise positioning or a confirmable destination where appropriate.

Allow sequential completion of simultaneous steps. For example, select an object, choose its destination, preview the result and confirm. Keep the selected item available while navigating. Explain mode changes and offer undo. If a physical skill is the actual subject of assessment, define the necessary skill explicitly and provide accessible assessment arrangements instead of silently marking an alternative as failure.

## Make targeting tolerant without making it unpredictable

Increase effective target area and separation, offer adjustable gain and stabilisation, and allow snapping or axis constraints for tasks that do not require free movement. Separate exploration from activation. Gaze landing on an object should not automatically trigger a consequential action; dwell needs adjustable timing, visible progress and a way to cancel.

Test dense layouts, overlapping targets, moving objects and targets close to the edge of the view. A large invisible hit area can select the wrong adjacent control. Stabilisation can reduce tremor but increase delay. Let people tune these behaviours in a safe practice area and restore a known configuration.

Provide a list or structured sequence of nearby or relevant objects when free aiming is a barrier. Include object names, states and available actions. Keep the list consistent with the world: it must not expose unavailable actions, hide the selected object or silently change order while a scanning user is choosing.

## Treat each input alternative as conditional

Voice requires speech, recognition, appropriate language and an acceptable acoustic and privacy setting. Eye tracking may fail or become tiring, and visual attention is not the same as intent. Hand tracking may not recognise atypical hands, movement or occluded positions. Head pointing requires tolerable head control. Touch and keyboard routes still require reachable hardware and meaningful focus order.

On recognition or tracking failure, retain the task state and offer a known alternative. Do not silently switch input modes and reinterpret the user's next movement. Explain which input is active and prevent the same action from firing twice when two input systems report it.

# 7 Movement orientation and comfort

## Offer movement choices with clear consequences

Apple's immersive-experience guidance recommends giving people control over immersion and supporting interaction without physical movement. Apply the broader design principle by reserving immersion for aspects of the experience that benefit from it and making a lower-immersion route available where feasible. Verify the implementation against the actual platform's behaviour. \[W10\]

Provide stationary interaction and a route that does not depend on walking, crouching, leaning or turning the body. For virtual travel, consider named destinations, teleportation, stepwise movement and optional continuous locomotion. Each option needs a usable selection method: ray-based teleportation alone still requires aiming.

Preview the destination and, where relevant, the arrival orientation. After moving, identify the new location and preserve a stable reference. Avoid a teleport that lands the person facing an unexpected wall or leaves essential controls behind them. Make backtracking and return to a known place easy.

For continuous movement, expose appropriate speed and turning options, and avoid forced acceleration, camera shake, camera roll or unexpected displacement. Keep essential task outcomes available when optional motion effects are reduced. Teleportation and snap turning are candidates to test, not guarantees of comfort.

## Build orientation into the environment

Use distinctive, meaningful landmarks and consistent spatial relationships. The BBC low-vision adaptation improved orientation by differentiating views, but similar entrance and garden treatments still caused confusion. This supports testing landmarks from the user's actual restricted view rather than judging a room from an overhead design image. \[B05, pp 8–10\]

Provide an on-demand answer to "Where am I?", "What is around me?" and "How do I get to my destination?". Make route information available without requiring a mental map of the whole scene. Give directional language a clear reference, such as relative to the user's current facing direction, and update it when that reference changes.

Do not use real-world inaccessibility as an unexamined interaction requirement. A virtual step, cobbled path or pit may suggest danger or exclusion even where no collision exists. Explain the available route, offer a direct route where the journey is incidental, and preserve exploration for people who want it. \[B01, B02\]

## Distinguish physical movement from virtual movement

Virtual recentering does not move a physical obstacle. An apparent virtual chair is not safe to sit on unless an appropriately verified physical seat is present. Label transitions between virtual travel and real movement. For room-scale activities, assess the swept space of the person's body, arms, mobility equipment and cables, not only the headset's location.

Treat boundary alerts as supplementary protection. Test whether the user can perceive them, understand their meaning and take the required action. Avoid game rewards that encourage crossing boundaries, sudden lunges or reaching through real furniture. Preserve access to mobility aids and assistance.

## Reduce motion burden and support stopping

Apple's motion-sickness guidance recommends reducing visual and unnecessary head motion and using available motion-reduction options. Treat these as ways to explore a more tolerable configuration, not a cure or a reason to continue through symptoms. The required head movements of an otherwise static interface also need assessment. \[W13\]

Provide a readily available pause that stops avoidable motion and audio stimulation, with a predictable recovery screen. Preserve world state and explain how resuming will behave. In multiplayer, a personal pause may not stop the shared world; provide a safe participation state and make that difference clear.

Test the complete motion pipeline on device. Frame rate, latency, tracking stability, scene motion, optics and individual susceptibility all affect the experience. A high average frame rate cannot establish comfort. Record discomfort and withdrawals alongside task success, rather than excluding those sessions from the findings.

# 8 Visual and nonvisual access

## Make contrast work in context

Test hands, pointers, focus indicators, objects, routes and text against every relevant background and lighting condition. Include transitions from bright to dark areas, occlusion, transparency and movement. The BBC findings show why one static colour cannot solve contrast across an entire scene. Allow object and background treatments to be adjusted independently. \[B01, B05\]

Use outlines, solid backplates or simplified materials where these help, and provide non-colour cues for meaning. Avoid making every object equally prominent: highlight the selected item and actionable content without erasing useful context. Offer reduced glare and brightness options alongside high contrast.

For conventional interface text, WCAG 2.2 specifies a minimum contrast ratio of 4.5 to 1, with 3 to 1 for qualifying large text; relevant non-text visual indicators have a 3 to 1 criterion with defined scope and exceptions. These are useful baselines for applicable UI. They are not a validated visibility model for stereoscopic objects or optical see-through displays. \[W16\]

## Support reading without posture or timing penalties

Let people adjust text size, position, distance, background and persistence. Provide a stable readable version of text on moving or distant objects. Reflow menus and instructions rather than clipping enlarged text. Keep focus and the current reading position when the view changes.

Do not require someone to lean across a gap or move their head excessively to read. Bringing content closer is useful only within comfortable optical and physical limits; enlargement and a separate reading view may be better. Test actual rendered legibility in the headset, including lens edges, aliasing, contrast changes and language expansion.

For signage, test discovery from multiple directions, heights and approach routes. Provide an accessible list of destinations or an equivalent query. The BBC signage changes left substantial difficulties, especially where reading and navigation had to happen together. Avoid making people read while moving. \[B05, pp 11–12\]

## Preserve context when magnifying

Offer an overview, a way to return to the previous scale and location, and access to critical alerts without searching outside the magnified view. Ensure targets remain selectable and that enlargement does not turn a simple menu into a repeated head-scanning task.

SeeingVR combined configurable visual and audio aids and was evaluated with 11 low-vision participants, who performed the study tasks more quickly and accurately with the tools. It supports offering combinations of aids rather than one fixed low-vision mode. It does not establish a universal best setting or blind access. \[E02\]

## Size content for the view and the optics

Specify viewing distance and angular size as well as world dimensions or interface units. A six-centimetre-wide target spans about 3.4 degrees at one metre but only 1.7 degrees at two metres. These are geometric examples, not minimum target sizes. Compare legibility and selection using the actual device, input and layout; do not transplant a pixel, point or centimetre threshold between platforms without its viewing assumptions.

Place frequent reading and interaction where the person can use their preferred neutral posture. Offer world-anchored, repositionable or view-following presentation as appropriate. A world-anchored panel can be hard to find; a head-locked panel can feel intrusive or move while being read. Test stability, discoverability and occlusion rather than choosing one anchoring rule for every task.

In conventional stereoscopic displays, the eye's focusing distance can differ from the depth indicated by binocular disparity. Experimental work has shown that this conflict can impair visual performance and increase fatigue. Avoid unnecessary extreme depth placement and repeated near-to-far shifts, follow device-specific optical guidance and offer a stable reading view. This evidence does not supply a universal comfortable depth range for every headset or user. \[E06\]

## Give the world usable meaning beyond pixels

Represent relevant objects with a meaningful name, type, state, location and available actions. Expose relationships needed for the task, such as which tool is selected, which doorway leads to the next room and whether an action succeeded. Keep decorative objects from overwhelming the navigable structure.

Support ordered navigation, object search and on-demand descriptions using the platform's accessibility mechanisms where available. A custom scene needs its own tested access design when those mechanisms do not expose it adequately. A label on a rendered texture is not a semantic object description.

Provide concise orientation first and detail on request. Let people interrupt, repeat or change description verbosity. Coordinate speech with task audio and user commands. For spatial tasks, descriptions must explain actionable relationships; "a red object" is insufficient if the user needs to locate and operate a valve.

Research with haptic and auditory cane interfaces demonstrates the possibility of nonvisual exploration. In the reported 2020 prototype study, seven of eight blind users completed the scavenger-hunt navigation activity. This is evidence of feasibility in a specific setup, not a requirement to reproduce cane use or proof that a commercial headset is accessible. \[E04\]

TetraLogical's seeing-disability guidance further supports queryable objects, adjustable presentation and recovery of viewing context. Use these as design directions and verify the whole journey with blind and low-vision users rather than treating visual simulation as a substitute. \[W05\]

# 9 Hearing speech and communication

## Preserve the meaning of sound

Inventory dialogue, narration, alarms, object sounds, navigation cues, turn-taking and ambient information that affects decisions. Provide text or another usable representation of the essential meaning, including who or what produced it and any task-relevant direction or urgency. A generic vibration cannot communicate all of those details.

Allow separate control of dialogue, background sound and effects. Offer mono output where supported without discarding directional meaning: retain an accessible direction label or equivalent cue. Test with audio muted, one audio channel unavailable and realistic background noise. Also test blind users' access when narration and spatial cues compete.

## Make captions usable within the scene

Provide accurate synchronised captions for speech and meaningful non-speech audio. Include speaker identification and off-screen speaker information when needed. Make captions discoverable before content starts, and offer size, contrast and position choices. Test caption reading while looking around and interacting, not just while facing a static test card.

BBC research comparing four subtitle behaviours for 360-degree video found a head-up presentation performed best in that study, while explicitly calling for further work on longer content. The practical lesson is to compare effort, obstruction, missed content and immersion across placements, rather than assume that subtitles attached to a world object will remain discoverable. \[E03\]

Meta's guidance recommends keeping captions visible, providing speaker attribution and backgrounds, and permitting placement adjustments. Its numerical positioning examples are platform design starting points. They should not be applied as universal distances or field-of-view limits across headsets, visual needs and content. \[W09\]

Separate live synchronised captions from a user-controlled history or transcript. Allow pause and replay for recorded content; for live interactions, make missed messages recoverable without implying that pausing the local display pauses other people. Review automatic caption errors for names, accents, terminology and simultaneous speakers. Do not present unverified transcription as authoritative in consequential instructions.

## Support sign language and non-speaking participation

Select sign languages with the intended audience; they are not interchangeable translations of a shared spoken language. Preserve visibility of hands, face and upper-body expression, with adjustable presentation and a placement that does not hide the task. Review signed content with fluent users. TetraLogical identifies both language access and readable presentation as necessary considerations. \[W06\]

For live social XR, establish whether the camera, tracking, avatar and network preserve the features needed to understand signing. If they do not, offer a usable video or other agreed communication route. Do not assume that hand-tracked avatar movement constitutes intelligible sign language.

Support text entry, prepared phrases, augmentative and alternative communication and text-to-speech where appropriate. Do not require speech to authenticate, ask for help, take a turn or exit. Preserve adequate time to communicate, and avoid showing communication aids or access settings to others without the user's choice.

## Keep social safety controls accessible

Provide reachable controls to mute, block, report and leave, along with control over interpersonal distance and unwanted contact. Make the effect clear: muting someone, hiding their avatar and leaving a shared session are different outcomes. Test moderation flows with the same input and output alternatives as the main activity.

Maintain accessible communication when a person changes input, pauses or removes the headset. A facilitator or collaborator should know that participation has paused without receiving private information about the reason. Treat these social and privacy provisions as product requirements to validate, rather than as findings established by the BBC sample.

# 10 Cognition learning and sensory experience

## Make possibilities and next steps explicit

Use consistent indicators for interactive objects and explain their actions. Decorative controls that look operable can create false expectations. Conversely, removing familiar detail may make a setting harder to interpret. The BBC cognitive work reports both the value of reducing spurious affordances and participants noticing missing environmental detail. Test what each detail communicates before removing it. \[B02\]

Offer an optional practice area with clear goals, immediate feedback and no penalty for mistakes. Teach one action at a time, while keeping help available later. Let people explore controllers and other input equipment before immersion when useful; reset the virtual starting state afterwards so practice does not accidentally change the task. \[B02, B05, B06\]

## Reduce memory and divided attention demands

Keep the current objective, progress and next action available on demand. Use the same names in prompts, controls, descriptions and feedback. Allow replay of demonstrations and instructions. Break complex actions into manageable steps without removing the ability to see the overall task.

Provide a recovery summary after interruption: what has happened, what remains selected and what the person can do next. Preserve entered information and completed work. Avoid restarting onboarding every time someone takes a break or changes input.

Give enough time to read, decide, move and communicate. Where timing is essential, document why and offer practice, alternative pacing or a comparable assessment route where possible. A countdown that is itself inaccessible does not provide meaningful warning.

## Make sensory content controllable

Separate essential information from optional animation, crowd activity, ambient sound, particles, haptics and notifications. Let users reduce these layers individually and access a calm starting configuration. Keep essential status understandable after optional effects are removed. TetraLogical similarly recommends control over non-critical content and accessible reminders of objectives. \[W08\]

Consider brightness changes, flashes, repetitive patterns, looming objects, sudden sounds, bass vibration and unexpected simulated touch. Test transitions as well as steady scenes. Analyse flashing and other hazardous content with appropriate specialist methods before participant exposure; an ordinary usability session is not a way to test whether a dangerous stimulus is tolerable.

## Respect expectations and emotional control

Preview heights, confinement, underwater scenes, rapid movement and other potentially distressing content in plain language. Offer choice and an accessible alternative where the experience's purpose permits it. Do not assume that a scene is reassuring because the designer finds it familiar.

Let people choose or adjust body representation where it matters, including hand appearance and the presence of mobility equipment. Test mismatch between visible hands and actual movement. Explain assistance before touching a person or moving their equipment, and agree a stop signal that does not rely on speech or sight. \[B01, B02\]

An in-experience quiet space should reduce stimulation and preserve control, but cannot substitute for stopping or removing a device when that is needed. Avoid making an exit itself theatrical, noisy, animated or dependent on completing another challenge.

# 11 Additional requirements for AR and mixed reality

## Distinguish the display and tracking conditions

Head-mounted video passthrough presents a camera-mediated view of the environment. Optical see-through overlays light onto a view of the real world. Handheld AR adds the demands of holding and aiming a screen. These arrangements create different visibility, occlusion, tracking and physical-workload conditions. Validate each supported mode independently.

For optical see-through devices, do not assume that a nominal black UI background can make the real scene opaque. For video passthrough, assess latency, image quality, camera occlusion and changes in brightness. In both cases, verify that essential information remains available against the actual environment rather than only an idealised screenshot.

## Reduce environmental setup demands

Explain required light, surfaces, space, camera permissions and connectivity before the person begins. Test cluttered and small spaces, reflective and low-texture surfaces, partial views and changing light. Apple describes surface detection and relocalisation as conditions that require clear guidance and recovery, and notes that prolonged device holding can cause fatigue. \[W14\]

Offer alternatives to repeated broad scanning, reaching around an object or walking a perimeter when these are not essential. Allow manual placement, an accessible list, a seated tabletop arrangement or a non-AR viewer where appropriate. If tracking cannot support a task reliably, say so and preserve work; do not repeatedly instruct the person to make an impossible movement.

TetraLogical's moving-disability guidance proposes recentering an object and offering selectable viewpoints so a mounted-device user can inspect it. Use these patterns when the goal is viewing the object, while keeping any real-world measurement or alignment task clearly separate. \[W07\]

## Handle anchors uncertainty and occlusion

Provide feedback when an object is placed, tracked, lost or repositioned. Allow recovery of off-screen objects without a physical search. After tracking resumes, avoid silently accepting a changed anchor as the same accurate location. Require revalidation before a placement is used for a consequential real-world action.

Use visual occlusion where it helps realism, but do not let it hide essential controls, instructions or alerts. Provide a discoverable overlay or nonvisual equivalent. An inspection mode may show an otherwise obscured object, but should make clear when the view no longer represents physical occlusion or actual scale.

Distinguish app-generated information from verified physical facts. An arrow over a doorway is not proof that the route is clear; a virtual outline is not proof that a machine is safe. For work involving real hazards, use a domain-specific safety assessment and independent controls rather than relying on an XR overlay alone.

## Keep attention compatible with the surroundings

Avoid tasks that require detailed reading or precise input while the person is moving through public space. Provide a stop-and-inspect mode, preserve progress and offer alerts in a form the user can perceive. Check whether headphones or overlays mask people, traffic, steps, doors or workplace alarms.

Use accessible routes and stopping places in location-based experiences. Do not award progress only for reaching a physically inaccessible coordinate or scanning a marker at one fixed height. Offer equivalent discovery mechanisms while preserving the activity's purpose.

For shared AR, verify that participants agree on the placement and meaning of shared objects even when their individual maps differ. Make corrections visible. Design permission and recording notices for users and bystanders, and minimise capture of private spaces. These are additional risk-based design recommendations; the supplied BBC research does not validate outdoor navigation or safety-critical AR.

# 12 Design redundancies and competing needs

## Specify redundancy at the level of meaning

For every essential message or action, record the information needed, the default route, alternatives, dependencies and the outcome if a route fails. Two sensory cues count as useful redundancy only if the person can understand and act on the remaining cue. Input redundancy must extend to selection, confirmation, correction and exit.

The following matrix gives implementation candidates. Select and test them with the intended users rather than enabling every channel by default.

| **Essential function**     | **Possible independent routes**                                                               | **Failure or conflict to test**                                                                      |
| -------------------------- | --------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| Find and choose an object  | Direct or ray selection; ordered object list; named voice command                             | All routes still requiring sight, exact aim or the same tracking system                              |
| Understand a warning       | Persistent text with meaning; speech; distinguishable haptic cue backed by retrievable detail | Colour-only coding; unclear vibration; audio masked by narration                                     |
| Navigate to a destination  | Visual landmarks; spoken route or location list; selectable destinations                      | Head turning required in every route; ambiguous arrival orientation                                  |
| Read or inspect content    | Resizable stable panel; read-aloud; accessible companion presentation                         | Enlargement hides controls; moving panel cannot be acquired; companion requires inaccessible pairing |
| Follow a conversation      | Audio; captions with attribution; appropriate sign-language or text route                     | Off-screen captions; signing cropped; communication lost when the user pauses                        |
| Pick up and move an item   | Direct grab; select then place; constrained movement controls                                 | Toggle state unclear; release inaccessible; object drops outside reach                               |
| Pause and recover          | Accessible persistent action; mapped switch or key; agreed facilitated stop                   | Every route depends on failed app tracking or on removing the headset unaided                        |
| Continue without immersion | Windowed or desktop interaction; accessible physical or assisted equivalent                   | Core decisions, social participation or achievements removed                                         |

## Test loss of a channel and combined needs

Run the essential journey with audio absent, haptics absent, one controller unavailable, tracking degraded and the supported nonvisual route active. These are engineering failure tests, not simulations of disability. Then validate real use with people who rely on those routes.

Test combinations deliberately. Captions plus magnification may cover the selected target; switch scanning plus a timeout may make confirmation impossible; a reduced-motion mode may suppress the only success cue. Test the most consequential combinations identified by research and dependency analysis, rather than assuming every option works in isolation.

## Resolve conflicts through control and clear priorities

High contrast and low glare should be separable. Magnification should retain an overview. Pointer smoothing should be adjustable and avoid changing discrete controls unnecessarily. Captions should offer a stable position and task-aware placement without moving unpredictably while being read. A calming mode should retain warnings and explain any remaining essential stimulation.

Do not quietly remove access features to recover performance. Reduce decorative quality first, and test that any adaptive rendering preserves text, focus indicators and nonvisual timing. If the system cannot maintain a usable experience, pause and explain the recovery options.

## Check whether an alternative merely moves the barrier

The BBC head-mounted switch scheme reduced hand requirements but retained head movement and press-and-hold. The chair-mounted scheme depended on moving the chair or body to aim. The rotate-and-forward scheme removed pointing but introduced sustained movement controls. Their value lies in showing why mappings should be adaptable, not in identifying one universal replacement controller. \[B04\]

For each alternative ask: what new physical, sensory, cognitive, privacy or setup demand has been introduced? Who controls it? Can it be changed during the task? What happens when it fails? Record the answers alongside the original barrier.

# 13 Software architecture and service design

## Maintain an accessible model of the experience

Keep the task state independent of the renderer and individual input devices. Store meaningful object identity, available actions, focus, selection, progress and messages so different presentations can use them. This makes a list-based route, narration, companion display and visual scene less likely to diverge.

W3C's XR requirements support semantics, input customisation, critical-message access, orientation and alternative presentation. The following architecture is a proposed way to operationalise those needs, not a W3C-mandated implementation. \[W01\]

Route input through named actions, validate an action once, update shared state, and generate appropriate visual, auditory, textual and haptic feedback from that state. Give asynchronous events clear priority. Keep focus stable when an alert appears, while making the alert discoverable and actionable. Avoid reading every moving object's state continuously.

## Make personalisation available from the beginning

Offer accessible setup before mandatory calibration or a timed tutorial. Use platform preferences where supported and sensible, while allowing app-specific adjustments. Let users preview settings, undo changes and recover defaults without losing their chosen input route. Make defaults understandable by function rather than by diagnostic labels.

Persist preferences appropriately across sessions, and test what happens after an update, device change, guest login or restored save. On shared devices, separate reusable access preferences from personal information and provide a clear reset between users. Do not overwrite another person's configuration without notice.

## Make the companion experience genuinely useful

A second screen can support setup, text entry, captions, observation or assistance, but introduces pairing, authentication, device availability and synchronisation dependencies. Test these explicitly. Allow the user to choose what is mirrored and who can control it. A facilitator view should distinguish a suggestion from an action performed on the user's behalf.

Keep the same task state and outcome across headset and companion modes. If changing mode requires leaving a session or losing work, document and address that cost. Do not assume that everyone owns a second device or has someone available to operate it.

## Privacy security and operational access

Explain collection of gaze, voice, movement, room maps and recordings in accessible language. Collect only what the product or agreed research requires, define retention and access, and avoid exposing disability-related settings to peers. Make consent changes and deletion requests usable through the supported access routes. Obtain specialist review where legal or sector obligations apply.

Include accessible purchasing, installation, sign-in, recovery, updates, troubleshooting and support. Publish actual tested capabilities, supported devices and known limits. "Supports accessibility" is less useful than a clear account of whether a person can complete setup, navigation, interaction, communication and exit with their input and output combination.

For venues, plan equipment inspection, charging, cleaning, spare compatible parts, staff training and escalation. Maintain a session reset that restores a known safe starting position without deleting the next user's required accommodations. The BBC session flow provides a useful arrival-to-debrief model, but each service needs its own current operating procedure. \[B09\]

# 14 Performance reliability and measurement

## Use the actual delivery pipeline

The BBC performance report investigated long-running thermal behaviour and repeated headset movement. It found that the test system could slow after sustained load and recognised the limits of a rig that did not exercise all rotational axes. These are useful lessons for endurance testing. Its historical claim that more than 90 frames per second establishes safety and comfort should not be used as a universal rule. \[B07\]

Choose a supported display mode and measure whether the application sustains its intended frame delivery. Meta's documentation illustrates frame budgets of approximately 13.9 ms at 72 Hz, 11.1 ms at 90 Hz and 8.3 ms at 120 Hz. These describe refresh intervals, not overall latency limits or guarantees of comfort. Distinguish newly rendered frames, compositor output and reprojection when reporting results. \[W15\]

Profile the production build on supported hardware under realistic load. Include complex scenes, captions, descriptions, assistive features, multiplayer, recording or mirroring when offered, network variation and a thermally warmed device. Measure frame-time distributions and spikes rather than relying only on average FPS. Record stalls, input-to-feedback delay, tracking failures and recovery behaviour.

## Preserve access when quality changes

Review dynamic resolution, foveated rendering, antialiasing and level-of-detail transitions for their effect on text and indicators, especially outside the visual centre or after gaze-tracking loss. Do not assume that an optimisation that looks acceptable to a developer is usable for someone who relies on peripheral vision or magnification.

Check captions, speech and haptics against the event they describe after loading delays and network interruption. A late success cue can provoke duplicate actions; a stale direction can send someone the wrong way. Keep critical controls responsive when background assets are loading.

## Combine repeatable tests with human evaluation

Use scripted tasks and captured input traces for regression, and hardware-in-the-loop testing where it measures behaviour the simulation cannot represent. Cover rotation as well as translation. Bench tests should establish technical confidence before participant exposure, but cannot establish comfort, comprehension, trust or physical fit.

Do not copy the BBC report's undervolting or improvised motion rigs into production operations without appropriate engineering review. The transferable method is to investigate sustained performance, repeat after material changes and understand what the test omits. \[B07\]

## Agree measurable targets before acceptance

For each essential task define completion, prohibited failure modes, allowed assistance and the relevant measures. Track time and errors, but also effort, discomfort, recovery, confidence and the value achieved. Report the denominator and access configuration for every result, including those who could not complete setup or withdrew.

For sickness assessment, a published instrument such as the VRSQ can support consistent measurement when used according to its scoring and administration method. Its original development involved 24 users doing target-selection tasks; it is not a universal safety threshold. Pair questionnaires with symptom reports and a stop protocol. Do not continue exposure to obtain a final score. \[E05\]

Use a small set of complementary measures. Record independent completion and completion with agreed assistance separately; count wrong actions, retries and recovery steps; measure time on task without penalising a deliberately slower access method; and ask about effort, control, understanding and value. Include body-area discomfort and time to first symptom where relevant. Report distributions and individual patterns, not only means.

Set product-specific numerical targets after formative research and a risk review. For example, define the maximum tolerable delay from the agreed stop input to a quiet paused state, then instrument and verify that transition under load. Do not invent a universal "accessible" completion time, discomfort score or participant success percentage. The criterion must reflect the task and the consequence of failure.

# 15 Test programme and acceptance criteria

## How to run the tests

The following tests are proposed acceptance procedures. Tailor thresholds to the task's consequences and the actual supported configurations before testing. "Pass" means the defined procedure and criterion were met in the tested conditions, not that all users will succeed. Mark unsupported cases explicitly; do not silently remove them from coverage.

For every test record build, device, OS, display mode, input, output, preferences, posture, environment, participant or bench-test role, procedure, observations, assistance and result. Capture unresolved issues and an owner. Use bench and expert checks first, then sessions with relevant users. Never deliberately provoke a hazardous failure in a participant session.

## T01 Entry setup and onboarding

**Procedure:** Start from the actual booking or installation route and a fresh or guest configuration. Enable the required access features before completing account, calibration and tutorial steps. Repeat with the intended alternative input and output routes.

**Accept when:** The person can discover the requirements and complete entry with the advertised support model. No required accommodation is trapped behind the interaction it replaces. Failed calibration offers a usable route or a clear supported limitation. Record any external help, even if brief.

## T02 Stop exit and physical recovery

**Procedure:** Rehearse stop, pause, quiet-space access and headset removal before exposure. Exercise the software paths in every major state, including loading and shared activity. Bench-test the fallback when the app or input stops responding.

**Accept when:** The person can initiate stop through their agreed accessible route, stimulation ceases as designed, and physical assistance is available where needed. No confirmation puzzle, forced motion or inaccessible menu blocks recovery. Release should be blocked by an unresolved failure of the agreed stop procedure.

## T03 Fit posture and sustained comfort

**Procedure:** Evaluate donning, adjustment, reading, interaction and removal with the full worn configuration and intended accessories. Check the person's normal seating or support. Repeat representative tasks over a participant-led duration with breaks and stop criteria.

**Accept when:** The intended tasks do not require unsupported or painful posture, unacceptable pressure or continued use through symptoms. Fit remains usable and optical clarity can be maintained. Record non-completers and duration to discomfort; do not average them away.

## T04 Physical handling and recovery

**Procedure:** Test unpacking, charging, connecting, identifying controls by touch where relevant, putting down and retrieving devices. Use a controlled simulation of a dropped or unreachable controller rather than creating a trip hazard. Include shared-device cleaning and reset operations.

**Accept when:** Each advertised independent action is achievable, and any assistance requirement is declared and workable. No recovery requires unsafe reaching, removal of an essential aid or accidental activation. Mounts and cables remain clear of mobility controls and exits.

## T05 Complete alternative input routes

**Procedure:** Run the essential journey separately with each supported input profile, including one-handed and switch routes where claimed. Include menus, world interaction, text entry, settings, errors, help and exit. Disable the default input so it cannot conceal missing functionality.

**Accept when:** All essential actions and feedback remain available without a hidden need for the default controller, gesture or speech. Completion has the same meaningful result. Record extra steps, effort and assistance as well as binary success.

## T06 Targeting precision and confirmation

**Procedure:** Select small, distant, adjacent, moving and partly obscured targets using the intended inputs. Test adjusted gain, target size, dwell and stabilisation. Include looking at an object without intending to activate it.

**Accept when:** Intentional selection is reliable at the agreed task level, adjacent controls are not activated unpredictably, and consequential actions can be confirmed or corrected. No essential target requires an unsupported degree of steadiness or a fixed gaze duration.

## T07 Holding timing and simultaneous actions

**Procedure:** Complete grab, drag, teleport, object transfer and timed decisions using toggle or sequential alternatives. Pause during a latched state, change input and resume. Test slow scanning and delayed response.

**Accept when:** The alternative removes the original sustained or concurrent demand, its current state is clear, and cancel or release remains available. Unnecessary time limits can be removed or adjusted. Essential timing has a documented reason and a tested access arrangement.

## T08 Reach height and balance

**Procedure:** Repeat the task seated, with relevant supports and across the intended range of height and reach. Retrieve virtual objects from the floor, overhead and behind the user through alternatives. Change posture and recenter.

**Accept when:** Essential content can be brought into a comfortable interaction zone without leaning beyond support or standing unexpectedly. Recentring does not misrepresent physical obstacles. Task progress and selected objects survive posture changes.

## T09 Way finding and return

**Procedure:** Navigate to named locations and return using visual and nonvisual routes. Test symmetric scenes, reverse approaches, off-screen destinations and interruption midway. Ask the person to explain where they are and what the next instruction means.

**Accept when:** The destination, route and arrival orientation are understandable, and a wrong turn can be corrected without restarting. Signage is not the only route to essential information. Guidance remains correct after recentering and virtual travel.

## T10 Nonvisual world interaction

**Procedure:** With blind participants and the intended nonvisual interface, locate, identify, select, operate and verify the state of objects. Include an unfamiliar scene, an error, a moving event and a change of location. Test task-relevant spatial relationships, not merely menu labels.

**Accept when:** The participant can understand and complete the essential task without visual intervention beyond the declared service model. Descriptions are timely, interruptible and sufficient. Critical objects and actions are reachable through the semantic or alternative interface.

## T11 Text contrast and visual discovery

**Procedure:** Inspect content in the actual display across backgrounds, lighting, distances, view positions and supported visual settings. Check enlarged text, long translations, focus indicators, hands, moving objects and signs approached from different directions. Include low-vision users.

**Accept when:** Applicable interface contrast criteria are met and users can discover and read essential content without forced posture or time pressure. Text and controls do not clip or disappear when enlarged. Meaning survives loss of colour discrimination.

## T12 Captions audio alternatives and signing

**Procedure:** Run content with audio muted, looking in different directions and performing the main task. Check captions, speaker attribution, non-speech information, history, playback control and signed content where provided. Test actual live communication latency and errors.

**Accept when:** Essential meaning remains understandable and presentation does not force an inaccessible search or obscure required actions. Fluent users can understand the signed content. Changes in view and immersion preserve the chosen communication route.

## T13 Understanding memory and interruption

**Procedure:** Ask new users to discover possible actions and complete a multi-step task. Introduce an ordinary interruption, then resume. Check current-objective access, reminders, explanations, repeated instructions and error recovery.

**Accept when:** The user can identify the next step and recover context using the product's intended support. Unplanned coaching is recorded as a failure of the independent route. Decorative affordances do not repeatedly mislead people into impossible actions.

## T14 Sensory settings and transitions

**Procedure:** Expert-review potentially hazardous stimuli first. Then test controllable brightness, sound, movement and haptics with relevant users under agreed exposure conditions. Preview transitions and exercise the calm configuration and return route.

**Accept when:** Optional stimulation can be reduced without losing essential meaning, settings work during use, and stop remains accessible. Unexpected threatening content is not introduced without the intended warning and choice. No participant is asked to tolerate escalating distress.

## T15 Locomotion and motion comfort

**Procedure:** Compare supported stationary, teleport and continuous-movement configurations where appropriate. Check head-turning demand, arrival orientation, camera effects and transitions. Collect baseline and post-task symptoms using the agreed method and record early stops.

**Accept when:** The intended task has a usable lower-motion route and no forced motion remains in essential controls. Comfort findings are reported by configuration and person, including failures. A technical performance pass does not override symptom-based failure.

## T16 AR visibility and environmental variation

**Procedure:** Test the claimed indoor or outdoor conditions, relevant lighting transitions, visual clutter, occlusion and mounted-device use. Inspect overlay contrast and essential messages against varied backgrounds. Bench-test conditions outside the supported envelope.

**Accept when:** Essential content remains accessible within the stated envelope, and unsupported conditions are identified before misleading guidance is given. The experience does not require unnecessary walking or camera sweeping. A fallback preserves the task where feasible.

## T17 Tracking loss anchors and permission failure

**Procedure:** In a controlled setup, interrupt tracking, obscure a camera, deny permissions and restore the session. Move or invalidate a relevant physical reference. Check selected objects, anchors, action confirmation and the user's orientation after recovery.

**Accept when:** Failure is communicated through usable channels, unintended actions do not occur, and consequential placements are revalidated. Work is preserved and recovery does not require the failed input. Restored tracking does not silently establish false physical certainty.

## T18 Settings persistence and combined configurations

**Procedure:** Combine high-impact settings such as magnification, captions, switch scanning and reduced motion. Change input during a task, restart, update or restore a session, and use guest reset. Check rollback after an unusable configuration.

**Accept when:** Settings remain compatible, persist as intended and do not remove the recovery route. Shared-device reset protects personal information without obstructing the next person's accommodations. No essential feature is quietly disabled by another setting.

## T19 Performance endurance and load

**Procedure:** Run repeatable production tasks on minimum supported hardware, with full access features and relevant mirroring or network load. Warm the system through a realistic operating period. Capture frame-time tails, missed frames, stalls, latency and thermal behaviour.

**Accept when:** The agreed device-specific performance budget and recovery behaviour are sustained. No inaccessible degradation of text, captions, input or critical messages occurs. Retest after material hardware, engine, driver, OS or content changes.

## T20 Social participation and protection

**Procedure:** Join, communicate, take turns, pause and rejoin with the supported communication modes. Test personal-space controls, blocking, reporting and leaving with alternative input. Include delayed text or augmentative communication.

**Accept when:** Participants can contribute to the same meaningful activity without being penalised for their access method. Safety controls are reachable and their effects are clear. Private access preferences and the reason for a pause are not exposed unnecessarily.

## T21 Channel loss and redundancy

**Procedure:** Remove one output or input dependency at a time, using bench checks before user validation. Test audio off, haptics off, unavailable controller and tracking degradation. Trace each essential warning and action to a functioning alternative.

**Accept when:** The remaining route conveys enough meaning to act and complete or safely stop the task. Apparent alternatives do not share an undisclosed failing dependency. Any unavoidable single point of failure is documented and mitigated appropriately.

## T22 Privacy assistance and companion control

**Procedure:** Review consent, recording indicators, preference visibility, mirroring, remote assistance and account recovery through each access route. Disconnect a companion device mid-task. Ask users to explain what is shared and who can act.

**Accept when:** People can make an informed choice, withdraw access through a usable route and distinguish their actions from a helper's. A companion failure does not expose data or strand the user without stop and recovery. Unnecessary sensitive telemetry is absent.

## T23 Service delivery and support

**Procedure:** Rehearse booking, arrival, fitting, a stop event, equipment fault, debrief, cleaning and preparation for the next user. Include an alternative experience and an accessibility support request. Use the real staff instructions and equipment.

**Accept when:** Staff can deliver the stated support consistently, explain limitations and handle recovery without improvising unsafe workarounds. The user can obtain help without the inaccessible channel that caused the problem. Reset leaves a known and appropriate starting state.

## T24 Comparable outcomes across modes

**Procedure:** Compare headset, adapted and non-headset routes against the same stated purpose. Review available decisions, content, creative options, learning outcomes, social participation, privacy and achievement recognition. Invite users to assess value as well as effort.

**Accept when:** An alternative preserves the essential outcome and agency, or any material difference is transparently justified and addressed. A video-only substitute does not pass an interactive decision task merely because its content is captioned.

# 16 Safe sessions release and ongoing improvement

## Prepare sessions around consent and control

Provide an accessible explanation of the activity, equipment, recording, support and right to stop. Agree a stop signal and how the researcher will respond. Establish the person's preferred communication and assistance before fitting the device. Let them inspect and practise with equipment, and check the starting scene before immersion. \[B06, B09, B10\]

The supplied health-and-safety notice lists broad exclusions involving age and medical conditions. It is a historical study artefact, not a current universal screening policy. Use current manufacturer information, the actual activity's risk assessment and appropriate professional advice where needed. Avoid turning a diagnosis alone into an unsupported blanket exclusion. Equally, do not waive a relevant device warning to achieve a recruitment target. \[B08, W11\]

Check the venue, seating, clearances, lighting and equipment, including accessible arrival and recovery space. Offer a calm preview and a low-demand start. Explain before handing over or moving an object. If someone reports symptoms, distress or asks to stop, stop the exposure and follow the agreed recovery procedure. Do not promise safety on the basis that the experience is virtual.

## Capture more than completion

The BBC feedback form covers handling controllers, wearing and removing the headset, navigation, boundary awareness and understanding interactive objects. Retain that whole-experience coverage, but offer accessible response formats, an open account of what happened and the option not to answer. Do not force a single impairment category or rely on facilitator interpretation of emotion. \[B11\]

Distinguish participant-chosen assistance, planned service support and unplanned rescue. Record whether a person could access the activity at all, complete the task, recover from error and achieve the intended value. Follow up on delayed discomfort where appropriate to the study design and consent, without treating a missing response as absence of symptoms.

## Prioritise barriers by consequence

Block release for unresolved inability to stop or recover safely, misleading safety-critical information, or a known severe failure in an advertised essential route. Prioritise other barriers by exclusion, task consequence, recurrence, cumulative effort and the quality of available alternatives. Low frequency does not make a high-consequence barrier acceptable.

Do not average an excluded subgroup into an acceptable overall score. Report configuration-specific outcomes and remaining uncertainty. Where an access need remains unsupported, make that limitation clear before purchase or participation and provide a meaningful alternative or a remediation plan.

## Require evidence at each delivery stage

| **Stage**               | **Required evidence**                                                                                             | **Accountable lead**                                             |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------- |
| Concept and procurement | Purpose, access-demand map, hardware accommodation limits, participant involvement and alternative-route strategy | Product owner with design and accessibility leads                |
| Prototype               | Observed barriers, physical fit findings, tested input alternatives and a working stop procedure                  | Design and research leads                                        |
| Integrated build        | End-to-end access routes, semantic content, settings interaction tests and performance results                    | Engineering and QA leads                                         |
| Release decision        | User evaluation, unresolved barriers, risk decisions, support procedures and accurate capability information      | Product owner with relevant safety and accessibility specialists |
| Operation and updates   | Accessible feedback, incident review, regression coverage and version-specific retesting                          | Service owner and engineering lead                               |

Name real owners in the project record. A platform limitation still needs a product decision: change the implementation, choose another device, narrow and disclose the supported use or provide a comparable route. It is not resolved by assigning it to the supplier without follow-up.

# 17 Worked example of an inclusive experience

## Inspecting and placing an object in a virtual museum

Assume the goal is to learn about an artefact, compare its features and place it in a chosen exhibition. This is a design example, not a tested product. The default concept asks users to walk to a shelf, grasp an object with both hands, rotate it to read small labels and place it on a distant plinth before a timer expires.

That concept combines holding, orientation, multiple input, reach, comprehension, timing and text barriers. A caption option alone would leave most of them intact. The following redesign preserves inspection and curatorial choice while removing incidental physical demands.

## Build the alternative routes into the task

At entry, the visitor can choose seated or standing presentation, configure input and output, and rehearse stop. The artefact can be selected in the world or from a named list. Selection opens an inspection state with a stable label, read-aloud, optional captions for narration and selectable viewpoints. Direct rotation remains available, but individual rotate controls and a reset view support other inputs.

The visitor chooses a destination from the room or a list of plinths. A preview identifies the destination and selected artefact; confirmation places it. Undo is available. The task does not require sustained grip, a second controller or reaching the floor. A dropped virtual object returns through an explicit retrieve action rather than disappearing or teleporting unexpectedly.

The layout uses distinctive landmarks and accessible location queries. Optional ambient sound and movement can be reduced. There is no timer unless time pressure is part of the stated purpose; if it is, provide an equivalent mode and make the difference clear. A desktop route supports the same artefact information, placement choices and shared exhibition.

## Validate what changed

Run [T05](#t05-complete-alternative-input-routes) and [T07](#t07-holding-timing-and-simultaneous-actions) to verify the complete input route; [T08](#t08-reach-height-and-balance) for reach; [T10](#t10-nonvisual-world-interaction) and [T11](#t11-text-contrast-and-visual-discovery) for object information; [T12](#t12-captions-audio-alternatives-and-signing) for narration alternatives; and [T13](#t13-understanding-memory-and-interruption) for understanding and recovery. Use [T18](#t18-settings-persistence-and-combined-configurations) and [T21](#t21-channel-loss-and-redundancy) to expose conflicts between settings and shared dependencies. [T24](#t24-comparable-outcomes-across-modes) checks whether the adapted and desktop routes preserve meaningful curatorial participation.

Then test the physical product and service through [T01](#t01-entry-setup-and-onboarding) to [T04](#t04-physical-handling-and-recovery) and [T23](#t23-service-delivery-and-support). A successful software redesign is incomplete if the visitor cannot fit the headset, enter their preferences or get assistance. Record any remaining limits in the access information before the visit.

# 18 Sources and evidence notes

Sources below distinguish supplied research materials from web guidance and supplementary empirical work. Web resources were reviewed on 28 October 2026. Page references for supplied PDFs use PDF page order, including covers. A source citation supports the associated finding or design rationale; it does not mean that the source tested every acceptance procedure in this handbook.

## Supplied research materials

**B01** [**Barriers Browser**](https://www.bbc.co.uk/accessibility/forproducts/xr/barriers)

BBC. Supplied Word document; undated. Canonical category descriptions, research scope and limitations. Original web address below.

**B02 Cognitive Barriers Deep Dive**

Jamie Knight and BBC Accessibility. Supplied cognitive-barriers-presentation.pdf, 67 pages. Observations, cognitive categories and environmental and facilitation adaptations.

**B03 Motor Barriers Deep Dive**

Jamie Knight and BBC Accessibility. Supplied motor-barrier-presentation.pdf, 88 pages. Motor categories and exploratory control schemes.

**B04 Switch Based Navigation in Virtual Reality Environments**

BBC UX and Design Accessibility. Supplied switch-access.pdf, 13 pages. Exploratory hardware and software mappings; especially pp 6–12. No single preferred scheme established.

**B05 Visual Impairment Barriers and Solutions**

BBC UX and Design Accessibility. February 2020. Supplied low-vision-adaptions.pdf, 13 pages. Exploratory findings; participant denominators and unfinished material limit quantitative interpretation.

**B06 User Testing in VR Quickstart Guide**

Jamie Knight and Oli with BBC Accessibility. Supplied how-to-guide.pdf, 68 pages. Recruitment, location, facilitation, controls and performance methodology. Historical equipment details require reassessment.

**B07 VR Performance Analysis and Tools**

BBC UX and Design Accessibility. December 2019. Supplied performance-testing.pdf, 8 pages. Endurance testing, thermal performance, motion rigs and their limitations.

**B08 Health and Safety Notes**

BBC research materials. Supplied health-safety-notice.pdf, 1 page. Historical HTC Vive study screening notice; not adopted as a universal exclusion policy.

**B09 VR Accessibility Session Flow**

BBC. Supplied session-flow-poster.pdf, 1 page. Arrival, media, interaction, observation and debrief model.

**B10 Virtual Reality Accessibility Research**

BBC Design and Engineering Accessibility. Supplied session-poster.pdf, 1 page. Participant information, support, stopping and recovery arrangements.

**B11 VR Feedback Form**

BBC research materials. Supplied feedback-form.pdf, 9 pages. Physical handling, comfort, navigation and interaction questions.

**B12 BBC AAD 2019 VR Barriers Research overview**

Jamie Knight and BBC Accessibility. Supplied vr-overview.pdf, 45 pages. Research goals and evolving recruitment and methodology; interim counts are not pooled with later results.

## Standards principles and platform guidance

**W01** [**XR Accessibility User Requirements**](https://www.w3.org/TR/xaur/)

W3C Accessible Platform Architectures Working Group. Working Group Note, 25 August 2021. User needs and requirements; explicitly not a baseline conformance standard. Relevant sections 3 and 4.

**W02** [**Introduction to XR Accessibility**](https://tetralogical.com/blog/2024/09/11/introduction-to-xr-accessibility/)

Joe Lamyman for TetraLogical. 11 September 2024. Frames the use of standards, XR requirements and BBC barriers as starting points alongside user research.

**W03** [**Introducing the Accessibility VRCs**](https://developers.meta.com/vr/blog/introducing-the-accessibility-vrcs/)

Oculus VR for Meta. 11 November 2020. Historical announcement; accessibility VRCs were described as recommendations at publication.

**W04** [**Get started with accessibility features on Apple Vision Pro**](https://support.apple.com/en-gb/guide/apple-vision-pro/tan426c48bdc/visionos)

Apple. Living support guide. Setup shortcuts and access to system and per-app settings. Verify behaviour on the deployed OS and app.

**W05** [**XR Accessibility for people with seeing disabilities**](https://tetralogical.com/blog/2024/09/19/xr-accessibility-for-people-with-seeing-disabilities/)

Joe Lamyman for TetraLogical. 19 September 2024. Queryable content, descriptions, magnification, personalisation and viewing context.

**W06** [**XR Accessibility for people with hearing disabilities**](https://tetralogical.com/blog/2024/10/01/xr-accessibility-for-people-with-hearing-disabilities/)

Joe Lamyman for TetraLogical. 1 October 2024. Signed content, audio information and alternative presentation.

**W07** [**XR Accessibility for people with moving disabilities**](https://tetralogical.com/blog/2024/12/09/xr-accessibility-for-people-with-moving-disabilities/)

Joe Lamyman for TetraLogical. 9 December 2024. Alternatives to physical movement, object viewpoints and configurable interaction.

**W08** [**XR Accessibility for people with thinking disabilities**](https://tetralogical.com/blog/2024/09/26/xr-accessibility-for-people-with-thinking-disabilities/)

Joe Lamyman for TetraLogical. 26 September 2024. Optional sensory content, objectives and recovery to a safe space.

**W09** [**Accessibility**](https://developers.meta.com/vr/design/accessibility/)

Meta Horizon OS Developers. Living design guidance; caption placement, synchronisation, attribution and customisation sections used here. Examples are platform guidance, not universal thresholds.

**W10** [**Immersive experiences**](https://developer.apple.com/design/human-interface-guidelines/immersive-experiences/)

Apple Developer. Human Interface Guidelines. Choice of immersion, stationary interaction and comfort. Platform-specific constraints require separate verification.

**W11** [**How to use your Apple Vision Pro safely**](https://support.apple.com/en-gb/118507)

Apple. Product-specific support guidance. Fit, breaks and stopping when unwell or uncomfortable. Not a clinical screening protocol for all XR.

**W12** [**About visual discomfort with Apple Vision Pro**](https://support.apple.com/en-gb/118476)

Apple. Product-specific support guidance. Fit, correction, display alignment, content positioning and interpupillary accommodation.

**W13** [**If you experience motion sickness while using Apple Vision Pro**](https://support.apple.com/en-gb/118497)

Apple. Product-specific support guidance. Reducing unnecessary head and visual motion and using available settings.

**W14** [**Augmented reality**](https://developer.apple.com/design/human-interface-guidelines/augmented-reality)

Apple Developer. Human Interface Guidelines. Handheld AR environment, placement, fatigue, surface detection and recovery considerations.

**W15** [**Missed frames and frame recovery**](https://developers.meta.com/vr/documentation/unity/os-missed-frames/)

Meta Horizon OS Developers. Updated 9 March 2026. Frame deadlines, missed frames and measurement. Used for frame-budget examples, not a claim about universal comfort or store acceptance.

**W16** [**Web Content Accessibility Guidelines 2.2**](https://www.w3.org/TR/WCAG22/)

W3C. Recommendation, 12 December 2024 edition. Scope and criteria 1.4.3 and 1.4.11 are relevant to the discussion of interface contrast.

**W17** [**Inclusive Design Principles**](https://inclusivedesignprinciples.info/)

Henny Swan Ian Pouncey Heydon Pickering and Léonie Watson. Principles for comparable experience, context, consistency, control, choice, prioritisation and value.

## Supplementary empirical research

**E01** [**Determining the effects of AR VR HMD design parameters on cervical spine joint torques**](https://pubmed.ncbi.nlm.nih.gov/38071785/)

Research article indexed in PubMed. Title in the original: Determining the effects of AR/VR HMD design parameters (mass and inertia) on cervical spine joint torques. PMID 38071785. Abstract reports 20 young adults and effects of mass, position and counterweights; findings do not establish a universal safety limit.

**E02** [**SeeingVR A Set of Tools to Make Virtual Reality More Accessible to People with Low Vision**](https://www.microsoft.com/en-us/research/publication/seeingvr-a-set-of-tools-to-make-virtual-reality-more-accessible-to-people-with-low-vision-2/)

Yuhang Zhao and colleagues. ACM CHI 2019. Evaluation with 11 low-vision participants. DOI 10.1145/3290605.3300341. Research toolkit and study findings, not a current commercial support guarantee.

**E03** [**Exploring Subtitle Behaviour for 360 Degree Video**](https://downloads.bbc.co.uk/rd/pubs/whp/whp-pdf-files/WHP330.pdf)

Andy Brown and colleagues for BBC Research and Development. White Paper WHP 330, cover dated 30 April 2018. Four subtitle behaviours evaluated; head-up presentation performed best under the study conditions. Longer-content suitability remained an open question.

**E04** [**Bringing virtual reality to people who are blind with an immersive sensory based system**](https://www.microsoft.com/en-us/research/blog/bringing-virtual-reality-to-people-who-are-blind-with-an-immersive-sensory-based-system/)

Microsoft Research. 2020 primary research account accompanying Virtual Reality Without Vision A Haptic and Auditory White Cane to Navigate Complex Virtual Worlds, CHI 2020. Reports seven of eight participants completing the prototype navigation activity.

**E05** [**Virtual reality sickness questionnaire**](https://pubmed.ncbi.nlm.nih.gov/29477332/)

Hyun K Kim Jaehyun Park Yeongcheol Choi and Mungyeong Choe. Applied Ergonomics 69, 2018, pp 66–73. Full title includes Motion sickness measurement index in a virtual reality environment. DOI 10.1016/j.apergo.2017.12.016. Initial development involved 24 users.

**E06** [**Vergence accommodation conflicts hinder visual performance and cause visual fatigue**](https://pmc.ncbi.nlm.nih.gov/articles/PMC2879326/)

David M Hoffman Ahna R Girshick Kurt Akeley and Martin S Banks. Journal of Vision 8(3), 2008. DOI 10.1167/8.3.33. Controlled stereoscopic-display experiments; not a universal headset-depth specification.
