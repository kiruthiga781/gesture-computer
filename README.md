# gesture-computer
Hand &amp; finger gestures via MediaPipe Hands — recognizes 21 landmarks per hand, enabling sign language letters, custom swipes, pinches, and holds Head movement via Face Mesh — nod, tilt, and directional looks mapped to actions Eye tracking via WebGazer.js 
Core feature set
Input modalities (all running in-browser via webcam, zero special hardware):

Hand & finger gestures via MediaPipe Hands — recognizes 21 landmarks per hand, enabling sign language letters, custom swipes, pinches, and holds
Head movement via Face Mesh — nod, tilt, and directional looks mapped to actions
Eye tracking via WebGazer.js — dwell-click (look at a button for 1–2 seconds to activate it), gaze-scroll, and directional control
Facial expressions via face-api.js — brow raise, smile, cheek puff, mouth open as discrete triggers
Communication outputs:

Text-to-speech with voice selection and speed control (Web Speech API, no server needed)
AAC-style symbol/picture board with gesture-to-tile selection
Live text window that types gesture-composed sentences
Clipboard export so users can "speak" into any other app
Key differentiators to build in
User-trainable gestures — let the user record their own gesture and bind it to any phrase or action. Someone with limited mobility might only be able to make 3–4 distinct movements; the system learns what those are.
Phrase prediction & autocomplete — powered by a small on-device LLM (like Phi-3 or TinyLlama via WebLLM), the system predicts the next word or whole sentence based on context and past usage patterns.
Emergency & priority mode — a single unmistakable gesture (like a sustained fist or eyes-closed hold) triggers a loud alert with a pre-set message for caregivers.
Offline-first PWA — all AI models cached locally after first load. Works without internet, installable on any device.
Caregiver panel — a shared secondary view (on another device or tab) that shows what the user is communicating in real time, with optional alerts.
Recommended build phases
Phase 1 — Foundation (working prototype): Hand gesture → text → TTS pipeline. Basic symbol board. User gesture training UI.
Phase 2 — Intelligence: AI phrase prediction, context memory, expression/head movement inputs.
Phase 3 — Polish & reach: Eye tracking, caregiver panel, offline PWA, multi-language support, WCAG 2.2 AA compliance throughout.
