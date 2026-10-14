# Mariem Kbaier

**AI Engineer** — computer vision, test-time adaptation, and local-first ML systems.
Tunis, Tunisia · [Portfolio](https://mariemkbaier.github.io/portfolio/) · [LinkedIn](https://linkedin.com/in/kbaier-mariem)

I build systems that hold up outside the demo: calibrated, evaluated against honest
baselines, and documented well enough to defend in a review.

---

### Selected work

**[Vision-Guided Pick-and-Place](https://github.com/mariemkbaier/cv-robotics-pipeline)** · Python, OpenCV, 6-DoF kinematics
End-to-end CV + robotics pipeline — camera to grasp, with no privileged information in
the loop: hand-eye calibration (AX = XB), 6D pose from PnP with ambiguity handling, IK
via damped least squares. The eval harness exists because an error in any one stage is
indistinguishable from the others at the gripper, so it attributes error to the right
stage. Every design decision, its alternative, and what it cost are recorded in
`DESIGN_NOTES.md`; twelve bugs found during development are now regression tests.

**[Test-Time Adaptation for Smart Buildings](https://github.com/mariemkbaier/TTA-Test-Time-Adaptation)** · Python, PyTorch
Cross-building activity recognition and occupancy estimation on WSU sensor data,
evaluating DIGA, PETAL and PeTTA under a deployable online protocol — both transfer
directions, chance baselines, paired bootstrap intervals. Found and documented that
stride-1 windowing under a random split inflates source macro-F1 to 0.998, and that
two of the three published methods do not adapt at all on this data. DIGA is the only
method with a significant gain (+1.7 macro-F1).

**[Meeting Assistant](https://github.com/mariemkbaier/meeting-assistant)** · Python, Whisper, RAG
Local-first multimodal meeting assistant: streaming ASR, retrieval over documents and
past meetings, live spoken Q&A, action-item extraction. Runs entirely on-device — no
audio or transcript leaves the machine.

---

### Currently

Working on evaluation methodology for domain adaptation — specifically, how much
reported transfer performance survives a leakage-free protocol.

### Reach me

kbaiermeryem@gmail.com
