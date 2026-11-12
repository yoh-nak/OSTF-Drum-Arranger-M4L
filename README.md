# OSTF Drum Arranger

**OSTF Drum Arranger** is a free Max for Live device for creating, generating, editing, capturing, arranging, reviewing, and exporting drum parts around the structure of a complete song using the **Open Song Timeline Format (OSTF)**.

Instead of treating drums as isolated MIDI clips, OSTF Drum Arranger works with the song itself: sections, roles, genre, tempo, meter, harmony, arrangement position, and other musical context.

Version 2.0 significantly expands the device beyond drum-pattern editing by integrating the current Composer-side songwriting, harmony, and review workflows while keeping the Drum Arranger workspace focused on drums.

---

## Main Features

- Section-aware drum arrangement
- Whole-song drum generation
- Section generation
- Pattern Banks A–H
- Step Editor
- Velocity editing
- Humanize tools
- Transition / Fill generation
- Start Phrase generation
- End Phrase generation
- Live MIDI Capture
- Dedicated Capture / Live I/O workspace
- MIDI export
- Send MIDI directly to Ableton Live
- Drum Rack / GM mapping
- MIDI Expression support
- Internal playback
- DAW Sync
- Section / Whole Song playback
- Loop and Loop Range
- Follow playback
- Compose Song
- Section Composer
- Harmony Studio
- Review Studio
- Working Key analysis
- Harmony Evidence
- Progression Library
- Genre-aware chord color
- Theory Guide
- Song Map editing
- OSTF Text support
- OSTF 4.x data-preservation workflow

---

# Song-Structure-Aware Drum Arranging

OSTF Drum Arranger works around the actual structure of the song.

Typical sections include:

- Intro
- Verse
- Pre-Chorus
- Chorus
- Bridge
- Solo
- Breakdown
- Drop
- Outro
- Custom OSTF sections

Each Section can maintain independent drum patterns and Pattern Banks while remaining associated with the song timeline.

The Section structure is shared with the OSTF song rather than being maintained as an unrelated drum-only arrangement.

---

# Drum Pattern Generation

Generate drum arrangements based on the current musical context.

Generation can consider:

- Genre
- Section role
- Section position
- Energy
- Song structure
- Current Pattern Bank
- Write Mode
- Existing locked notes
- Neighboring musical context
- Transition position

Generation is available at several levels.

### Generate Section

Generate the selected Section while preserving the rest of the song.

### Generate Whole Song

Generate drum parts across the complete OSTF song structure.

The Whole-Song workflow can consider different roles and energy levels for different Sections instead of applying one identical pattern across the entire song.

### Per-Row Generation

Individual drum lanes can also be regenerated independently.

---

# Pattern Banks

Every Section supports multiple independent pattern ideas.

Available Banks:

- A
- B
- C
- D
- E
- F
- G
- H

Banks make it possible to keep several drum interpretations for the same Section without losing the current arrangement.

Patterns can also be copied between Banks.

---

# Step Editor

The built-in Step Editor provides direct drum-pattern editing.

Supported grid resolutions include:

- 1/1
- 1/2
- 1/4
- 1/8
- 1/16
- 1/32
- 1/64
- 1/128
- Triplet

Editing includes:

- Note placement
- Velocity
- Fine hits
- Solo
- Mute
- Per-row generation
- Bar copy
- Bar paste
- Duplicate to next bar
- Lock protection
- Clear Solo / Mute

The editor can display different bar ranges while keeping the Section length owned by the OSTF song structure.

---

# Velocity Mode

Velocity Mode provides dedicated control over drum dynamics.

Velocity data can be edited independently of note placement.

This makes it possible to retain the pattern rhythm while reshaping accents, ghost-note behavior, and performance dynamics.

---

# Humanize Mode

Humanize Mode can introduce controlled performance variation.

Humanization can affect elements such as:

- Velocity
- Timing
- Accent balance
- Repetition feel

The goal is not to randomize the pattern blindly, but to make programmed drums feel less mechanically identical.

---

# Transition / Fill Generation

OSTF Drum Arranger includes dedicated transition tools.

Available phrase-generation workflows include:

- Transition / Fill
- Start Phrase
- End Phrase

These can be used without rebuilding the complete Section.

Typical use cases include:

- Verse → Chorus
- Pre-Chorus → Chorus
- Chorus → Verse
- Breakdown → Drop
- Bridge transitions
- Intro pickup
- Outro ending
- Section-opening fills

---

# Capture / Live I/O

Version 2.0 includes a dedicated **Capture / Live I/O** mode.

This workspace is separate from the Step, Velocity, and Humanize editing modes.

It provides both:

- MIDI Output
- Capture from Live

---

## Capture from Ableton Live

Selected MIDI clips can be captured directly from Ableton Live.

Captured MIDI is displayed in a drum-oriented piano-roll view.

Workflow:

1. Select a MIDI clip in Ableton Live
2. Open Capture / Live I/O
3. Capture the selected Live MIDI clip
4. Select a source range
5. Choose the destination OSTF Section
6. Choose the destination bar
7. Select the Write Mode
8. Review the assignment
9. Commit the selected range to the Drum Track

The source Live clip remains unchanged.

Commit includes a confirmation workflow so the destination Section, Bank, bar position, range, and Write Mode can be reviewed before writing.

---

# MIDI Output

The current Drum arrangement can be sent back to Ableton Live.

Output options include:

- Current Section
- Whole Song
- Active Bank
- Arrangement destination
- Session destination where supported
- DAW-synchronized placement
- Live Bar / Beat placement

You can either:

- Send MIDI directly to Live
- Export Standard MIDI

---

# MIDI Expression

MIDI Expression follows a common Arranger policy.

When **MIDI EXPRESSION** is enabled, supported non-note MIDI information is included together with note output where applicable.

There is no separate workflow requiring users to choose between a “notes only” mode and another full-MIDI mode.

The common MIDI Expression switch acts as the master policy.

---

# Drum Rack and MIDI Mapping

OSTF Drum Arranger supports both standard drum layouts and Ableton Drum Rack workflows.

Supported mapping workflows include:

- GM16
- Drum Rack
- Automatic scanning
- Manual mapping
- Pad Routing
- MIDI Learn

Drum lanes can represent roles such as:

- Kick
- Snare
- Clap
- Closed Hi-Hat
- Open Hi-Hat
- Pedal Hi-Hat
- Tom
- Rim / Side Stick
- Crash
- Ride
- Shaker
- Tambourine
- Cowbell
- Percussion
- FX / One-shot
- Custom
- Unassigned

Mapping can be adapted to different Drum Rack layouts without changing the musical role of the generated drum part.

---

# Playback

Playback options include:

- Section
- Whole Song
- Stop
- Loop
- Loop Range
- Follow

When Loop is enabled without a custom Loop Range, the currently selected playback scope is repeated.

For example:

- SECTION + LOOP → loop the current Section
- WHOLE SONG + LOOP → loop the complete song
- LOOP RANGE → loop the explicitly selected range

Playback can use:

- Internal playback
- DAW Sync

The current Section and playback position are visually followed during playback.

---

# Composer Workflow

Version 2.0 integrates the current left-side songwriting workflow from **OSTF Composer v3.0**.

The Drum Arranger keeps its own drum-specific right workspace, while the left side provides shared composition and harmonic tools.

---

## Compose Song

Compose Song can generate and explore chord progression ideas across the song structure.

Generation can consider:

- Genre
- Mood
- Harmonic Color
- Harmonic Depth
- Pattern Focus
- Variation
- Section roles
- Local Working Keys
- Neighboring progressions
- Song structure

Ideas can be generated, reviewed, auditioned, and applied without requiring the Drum Arranger to become a full voicing editor.

---

# Section Composer

Section Composer provides Section-level harmonic editing and generation.

It uses the current Composer-side:

- Progression Library
- Genre Context
- Genre Chord Color
- Working Key logic
- Harmony Evidence
- Theory-aware suggestions

The current Progression Library includes a large set of theory-derived and genre-aware progression patterns.

---

# Harmony Studio

Harmony Studio provides song-wide harmonic analysis and editing support.

It can work across multiple Sections and supports selection ranges spanning Section boundaries.

Features include:

- Chord progression overview
- Multi-chord selection
- Current Section selection
- Whole Song selection
- Harmonic-function analysis
- Tension / resolution analysis
- Suggestions
- Theory view
- Theory Map
- Development tools
- A/B comparison workflows

Selected chords use the same selection-state behavior as the current OSTF Composer implementation.

---

# Review Studio

Review Studio provides a dedicated workflow for evaluating existing harmony rather than immediately replacing it.

It can analyze musical context and generate review ideas based on:

- Harmonic function
- Working Key
- Progression context
- Section role
- Harmony Evidence
- Genre context
- Tension and resolution

Review Studio is useful when a progression is already mostly complete and the goal is to identify possible improvements rather than generate an entirely new progression.

---

# Working Key and Harmony Evidence

OSTF Drum Arranger v2.0 includes the Composer-side Working Key and Harmony Evidence systems.

These are used by Composer-related workflows to interpret harmony in context.

This is especially useful for:

- Local tonal centers
- Modal sections
- Borrowed harmony
- Section-to-section harmonic movement
- Genre-dependent harmonic interpretation

---

# Theory Guide

The left-side editor includes visual theory assistance for chord and scale context.

Theory information is intended as composition support rather than a restriction on what can be entered.

---

# Song Map

Song-level timeline information can be edited from the left workspace.

Supported contextual data includes:

- Key
- Tempo
- Meter

Section-local information can coexist with global song information where supported by the OSTF document.

---

# OSTF Support

OSTF Drum Arranger was originally developed around **OSTF 3.5** and now includes the Composer-side Core/Adapter behavior required to preserve and work with compatible **OSTF 4.x** documents.

Version 2.0 can preserve linked OSTF information such as:

- Song structure
- Section data
- Tempo
- Meter
- Key information
- Timed scale information
- Lyrics
- Imported tracks
- Other compatible timeline data

Complex OSTF data is no longer blanket-locked simply because additional non-drum information is present.

The Drum Arranger modifies its relevant drum data while attempting to preserve surrounding OSTF song information.

---

# OSTF Text

OSTF Text workflows are available for exchanging OSTF song information in text form.

The Drum Arranger retains its own Drum-specific import workflow so that a target Drum Track can be selected when appropriate.

---

# Undo and Editing

Editing tools include:

- Undo
- Redo
- Add Section
- Duplicate Section
- Delete Section
- Move Section
- Split
- Transpose
- Copy Bar
- Paste Bar
- Duplicate to Next
- Clear Solo / Mute
- Pattern Bank copy
- Lock protection

---

# English User Interface

The released device uses an English interface.

OSTF song content itself can still contain other languages.

For example:

- Song titles
- Lyrics
- Section names
- Metadata

are preserved where supported.

---

# Requirements

- Ableton Live
- Max for Live
- A compatible version of Max included with or supported by Ableton Live

OSTF Drum Arranger is distributed as an `.amxd` Max for Live MIDI device.

---

# Installation

1. Download `OSTF_Drum_Arranger_v2.0.amxd`
2. Place the file in your preferred Max for Live device folder
3. Open Ableton Live
4. Drag OSTF Drum Arranger onto a MIDI track
5. Click **Open** to open the full editor
6. Open an OSTF file or create a new song
7. Create or apply a song structure
8. Generate, edit, capture, arrange, review, and export drum parts

---

# Open Song Timeline Format

OSTF Drum Arranger is built around the **Open Song Timeline Format**.

OSTF is an open format for describing complete song structure and musical information, including:

- Sections
- Harmony
- Melody
- Lyrics
- MIDI notes
- Performance information
- Arrangement data
- Timing
- Tempo
- Meter
- Key maps
- Scale information
- Other song-level information

OSTF Drum Arranger focuses on the drum-arrangement workflow while preserving the surrounding song data whenever possible.

OSTF 3.5:

https://github.com/yoh-nak/Open-Song-Timeline-Format-3.5

---

# Project Philosophy

OSTF Drum Arranger is not intended to replace a dedicated drum instrument, sampler, or high-end drum library.

Its role is primarily:

- Composition support
- Drum arrangement
- Song-structure-aware editing
- MIDI capture
- Pattern experimentation
- Harmonic context
- OSTF integration
- Ableton Live integration

Your preferred Drum Rack, drum instrument, sampler, or external sound source remains responsible for the final sound.

---

# Version 2.0

Version 2.0 is a major workflow and architecture update.

Highlights include:

- Dedicated Capture / Live I/O mode
- Improved Live MIDI capture
- Review-before-commit Capture workflow
- Improved Standard MIDI export
- Common MIDI Expression output policy
- Improved Drum Rack and routing workflow
- Pattern Banks A–H
- Section and Whole-Song generation
- Transition / Fill generation
- Start Phrase generation
- End Phrase generation
- STEP / VELOCITY / HUMANIZE modes
- Stable Section / Whole Song playback
- Loop and Loop Range
- Playback Follow
- Improved Section synchronization
- Improved state recovery after New / Template Apply / Capture operations
- Composer v3.0 Compose Song integration
- Composer v3.0 Section Composer integration
- Harmony Studio
- Review Studio
- Working Key analysis
- Harmony Evidence
- Current Progression Library
- Genre Context
- Genre Chord Color
- Theory Guide
- Song Map
- OSTF 4.x preserve/edit behavior
- Improved Host State / Lifecycle handling
- Improved device-view loading behavior
- English user interface

The left Composer workspace is aligned with OSTF Composer v3.0 while the right side remains dedicated to the Drum Arranger workflow.

Composer-specific right-side Voicing Studio, Composer Capture / Output, and Composer DAW Sync are intentionally not included because OSTF Drum Arranger maintains its own drum-specific right workspace and I/O workflow.

---

# Support Development

OSTF Drum Arranger is available for free.

If you find the project useful and would like to support continued development:

**Buy Me a Coffee**

https://buymeacoffee.com/yohsukenak

Your support helps with continued development of:

- OSTF
- Max for Live devices
- Documentation
- Testing
- Music-production utilities
- Composition and arrangement tools

---

# Repository

OSTF Drum Arranger for Max for Live

https://github.com/yoh-nak/OSTF-Drum-Arranger-M4L

---

# License

Please refer to the license information included in this repository.

---

# Author

Developed by **yoh-nak**

Open Song Timeline Format / OSTF Max for Live Project
