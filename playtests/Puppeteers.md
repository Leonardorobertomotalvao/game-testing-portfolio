# Puppeteers — Playtest Report

**Tester:** Leonardo Roberto  
**Test date:** 2026-10-06  
**Platform:** Windows PC  
**Build / Version:** Not provided  
**Test type:** General playtest / QA feedback

## Test Environment

- **CPU:** AMD Ryzen 5 5500
- **GPU:** NVIDIA GeForce RTX 5060 8 GB
- **RAM:** 16 GB DDR4 3200 MHz
- **Resolution:** 1080p / 1440p
- **Operating System:** Windows

## Summary

Puppeteers was generally lightweight to run, but I noticed stuttering shortly after starting the game even on this hardware.

The main issues found during the session were related to player guidance and collision. Objectives were not always clear, environmental interaction felt limited, and some walls or objects did not appear to have proper collision.

The notebook was the main meaningful environmental interaction I found during the test. The experience would benefit from clearer guidance, more environmental interaction and stronger feedback to help the player understand what to do next.

---

## Issue 01 — Stuttering at the beginning of the game

**Category:** Performance  
**Severity:** Medium  
**Frequency:** Observed during the beginning of the session

### Description

The game showed noticeable stuttering shortly after starting, despite running on hardware that should be more than capable of handling the game.

### Steps to reproduce

1. Launch the game.
2. Start a new session.
3. Move around and play through the opening section.
4. Observe frame pacing and responsiveness during the first moments of gameplay.

### Expected result

The opening section should run smoothly without noticeable stuttering on supported hardware.

### Actual result

Noticeable stuttering occurred during the beginning of the game.

### Notes

The game otherwise appeared relatively lightweight during the test.

---

## Issue 02 — Missing or inconsistent collision

**Category:** Collision / Level Geometry  
**Severity:** High  
**Frequency:** Observed multiple times

### Description

Some parts of the environment did not appear to have proper collision. It was possible to move through certain walls or objects that visually looked solid.

### Steps to reproduce

1. Move around the environment.
2. Approach walls and solid-looking objects.
3. Continue moving against different surfaces.
4. In some locations, the player can pass through geometry instead of being blocked.

### Expected result

Walls and solid environmental objects should prevent the player from moving through them.

### Actual result

Some environmental geometry could be crossed or did not provide the expected collision.

### Impact

This can break immersion, allow the player to enter unintended areas and make it harder to understand which parts of the environment are meant to be accessible.

---

## Issue 03 — Objectives are not always clear

**Category:** Gameplay / Player Guidance  
**Severity:** Medium  
**Frequency:** Recurring during the session

### Description

The game does not always make the current objective clear. At some points, I had to guess what I was supposed to do next.

### Expected result

The player should receive enough visual, textual or environmental guidance to understand the next objective without excessive trial and error.

### Actual result

Progression could feel unclear because there was limited guidance explaining the next action.

### Suggested improvement

Consider using clearer objective prompts, environmental cues, short tutorial messages or additional contextual feedback.

---

## Issue 04 — Limited environmental interaction

**Category:** Gameplay / UX  
**Severity:** Low to Medium

### Description

Environmental interaction felt limited during the test. The notebook was the main meaningful object I found that the player could interact with.

### Expected result

Interactive elements should be clear and provide enough feedback to support exploration and progression.

### Actual result

There were few obvious interactions, which made parts of the environment feel less responsive and also contributed to uncertainty about progression.

### Suggested improvement

Additional interactive objects, clearer interaction feedback and more environmental responses could make exploration feel more intentional.

---

## Player Guidance and Presentation

I felt that the game could benefit from more guidance during the opening section.

Possible improvements include:

- a short introduction to the basic controls;
- clearer explanation of the first objective;
- more contextual prompts when the player is stuck;
- additional dialogue or environmental storytelling;
- clearer indication of which objects can be interacted with.

These changes could reduce the amount of guessing required from a new player while keeping the atmosphere and exploration intact.

---

## Developer Follow-up

After receiving the feedback, the developer acknowledged that player guidance and environmental storytelling still needed work.

The developer also mentioned that performance and collision-related problems had been especially noticeable on Intel GPUs and asked for the test PC specifications.

This test was performed using an **NVIDIA GeForce RTX 5060 8 GB**, so the stuttering and collision observations documented here were not produced on an Intel GPU.

---

## Final Assessment

The core concept was interesting, but the playtest revealed areas that could significantly improve the first-time player experience.

The highest-priority items from this session were:

1. Collision consistency
2. Clarity of objectives and player guidance
3. Initial stuttering / frame pacing
4. Environmental interaction

This report reflects observations from a single playtest session and is intended as constructive QA feedback for development.
