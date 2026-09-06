# Theatre Agent

**Build complete Ableton Live theatre sessions from audio files and cue instructions.**

Theatre Agent is a desktop application designed to turn the technical process of building an Ableton Live theatre session into a simple cue-based workflow.

Import your show's audio files, define what each cue should do, and Theatre Agent builds the Ableton Live project for you — including track allocation, routing, levels, fades, automation, looping, EQ, and cue-to-cue playback behavior.
## Interface

### Cue Editor

![Theatre Agent cue editor](theatre-agent-cue-editor.png.png)

### Cue List

![Theatre Agent cue list](theatre-agent-cue-list.png.png)
## The Problem

Ableton Live is powerful enough to run complex theatre playback, but building a show can involve a large amount of repetitive technical work.

Sound designers and operators may need to manually create tracks, place audio, configure outputs, set levels, program fades and automation, manage overlapping cues, and maintain playback behavior across an entire show.

For experienced Ableton users, this takes time.
## What Theatre Agent Can Build

Theatre Agent translates cue-level instructions into a structured Ableton Live session.

It currently supports:

- Automatic track allocation
- Main and monitor output routing
- Custom output lanes with matching automation tracks
- Per-cue playback levels
- Fade-in and fade-out automation
- Multiple fade trigger behaviors
- Overlapping cues
- Persistent playback across cues
- Run-with-previous / linked cue behavior
- Looping with automatic Warp configuration
- Per-cue low-cut and high-cut EQ automation
- Dedicated automation-only cues
- CUT / stop cues
- Selective track stopping and full-stop behavior
- Automatic scene creation and expansion
- Automatic cue naming and organization
- Multi-file and folder import
- Audio preview
- Cue reordering
- Automatic generation of the final Ableton Live project

The generated project opens directly in Ableton Live and remains fully editable by the sound designer or operator.

For theatre professionals who don't know Ableton deeply, it can make the software difficult to use at all.

Theatre Agent separates the creative decision from the technical implementation:

**You define what should happen. Theatre Agent builds the session.**
## How It Works

### 1. Import the show's audio

Add individual audio files, drag and drop multiple files, or import an entire folder.

### 2. Define each cue

Choose what should happen when the cue is triggered — output, level, fades, looping, EQ, playback behavior, and other cue-specific instructions.

### 3. Build

Theatre Agent processes the complete cue sequence and builds the required Ableton Live session automatically.

### 4. Open in Ableton Live

The generated project contains the tracks, scenes, audio clips, routing, automation, cue logic, and organization required by the show.

The session remains a normal, fully editable Ableton Live project.
## Demo

### Theatre Agent Workflow

From imported audio files to a configured theatre cue sequence and generated Ableton Live session.

[▶ Watch the Theatre Agent workflow demo](demo/Theatre_Agent_Demo_01_Cropped_MUTED.mp4)

### Generated Ableton Live Result

A walkthrough of the generated Ableton Live session, including cue placement, track allocation, routing, automation, and playback logic.

[▶ Watch the generated Ableton Live session](demo/Theatre_Agent_Demo_02_Ableton_Cropped_MUTED_FIXED.mp4)
## Generated Ableton Live Session

TheatreAgent converts cue instructions into a structured Ableton Live session, automatically handling track allocation, routing, automation lanes, and cue placement.

![Generated Ableton Live session](generated-session.png)

This example shows a generated theatre session with main and monitor playback, paired automation tracks, and a dedicated cut cue.

## Engineering Highlights

- Generates valid, editable `.als` sessions for Ableton Live 11
- Maintains playback state across cues, including overlapping sounds
- Allocates available playback tracks automatically when cues overlap
- Keeps paired AUTO tracks aligned with each playback cue
- Builds automation for fades, levels, routing changes, and EQ
- Expands the session dynamically when more scenes are needed
- Supports custom output lanes while preserving the existing session structure
- Includes a PySide6 desktop interface for building sessions without Ableton expertise
## Built With

- Python
- PySide6 / Qt
- Ableton Live 11
- Mutagen for audio-file metadata and MP3 support
- PyInstaller for desktop packaging
## Project Status

TheatreAgent is a working desktop prototype.

It can turn a set of theatre audio cues into a structured Ableton Live 11 session with playback tracks, automation, routing, fades, looping, EQ, and cut cues already prepared.

The current focus is further testing, workflow refinement, and preparing the tool for real-world use by theatre sound professionals.

The prototype is currently being tested with feedback from local theatre sound designers.
