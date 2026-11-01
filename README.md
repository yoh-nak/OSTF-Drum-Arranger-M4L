# OSTF Drum Arranger

**OSTF Drum Arranger** is a free Max for Live device for creating, editing, capturing, arranging, and exporting drum patterns using the **Open Song Timeline Format (OSTF)**.

It is designed for producers, composers, songwriters, and arrangers who want to build drum parts around the actual structure of a song rather than working only with isolated MIDI clips.

The device supports **OSTF 3.5** and works with song sections such as Intro, Verse, Pre-Chorus, Chorus, Bridge, Outro, and custom sections.

---

## Features

### OSTF 3.5 Support

- Designed for OSTF 3.5
- Reads song structure directly from OSTF files
- Uses OSTF-standard song, section, tempo, genre, note, drum mapping, and arrangement data
- Preserves existing OSTF information when editing drum arrangements
- Does not require Drum Arranger-specific vendor extensions for normal OSTF data
- Maintains compatibility with supported OSTF 3.x files where possible

---

## Section-Based Drum Arranging

Drum patterns are organized around the actual sections of the song.

You can move between sections such as:

- Intro
- Verse
- Pre-Chorus
- Chorus
- Bridge
- Outro
- Custom OSTF sections

Each section can contain its own independent drum patterns and Pattern Banks.

The drum arrangement stays synchronized with the song structure stored in the OSTF file.

---

## Drum Pattern Generation

Generate drum patterns based on the current song section and musical context.

Controls include:

- Genre
- Section type
- Generation style
- Pattern feel
- Note density
- Replace / generation behavior
- Bar range
- Whole-section generation
- Whole-song generation

Individual drum rows can also be regenerated independently.

---

## Step Editor

The built-in drum Step Editor provides direct control over the drum pattern.

Supported grid resolutions:

- 1/1
- 1/2
- 1/4
- 1/8
- 1/16
- 1/32
- 1/64
- 1/128
- Triplet grid

You can edit:

- Note placement
- Velocity
- Fine hits
- Drum rows
- Solo
- Mute
- Lock
- Per-row generation
- Per-row clearing

Playback feedback highlights the currently sounding drum row and active step positions.

---

## Velocity and Humanize

Dedicated editing modes are available for:

- Velocity
- Timing variation
- Humanization
- Performance variation

This allows generated patterns to be adjusted from rigid programmed drums toward more natural performances.

---

## Pattern Banks

Each OSTF section can contain multiple independent drum pattern ideas.

Pattern Banks:

- A
- B
- C
- D
- E
- F
- G
- H

You can quickly compare alternate patterns while keeping them associated with the same OSTF section.

Patterns can also be copied between Banks.

---

## Fill Generation

Create fills for transitions and section endings.

Fill tools can be used to add variation without rebuilding the full drum pattern.

Useful for transitions such as:

- Verse to Chorus
- Pre-Chorus to Chorus
- Chorus to Verse
- Bridge transitions
- Final section endings

---

## Phrase Compare

Compare generated drum candidates before committing them to the arrangement.

Phrase Compare helps evaluate alternative patterns while preserving the current pattern until a candidate is adopted.

This is useful when experimenting with different drum ideas without losing the existing arrangement.

---

## Live MIDI Capture

OSTF Drum Arranger can capture drum MIDI directly from Ableton Live.

The Capture workflow is designed around visually selecting musical bars.

### Capture Workflow

1. Select a MIDI source in Ableton Live
2. Capture MIDI into OSTF Drum Arranger
3. Captured MIDI is displayed as individual bar cards
4. Select one or more source bars
5. Assign those bars directly to an OSTF section

Selection supports:

- Click
- Shift + Click
- Ctrl / Cmd + Click
- Drag selection
- Shift + Drag
- Select All
- Clear Selection

Captured source MIDI remains unchanged.

The same selected bars can be assigned to multiple OSTF sections.

---

## Drum Rack and MIDI Mapping

OSTF Drum Arranger includes drum mapping tools for both standard MIDI drum layouts and Ableton Drum Rack workflows.

### Supported Workflows

- GM16
- Drum Rack
- Manual MIDI mapping
- Automatic mapping
- Drum Rack scanning
- Pad routing
- MIDI Learn

Each drum sound can be assigned a generator role such as:

- Kick
- Snare
- Clap
- Closed Hi-Hat
- Open Hi-Hat
- Tom
- Rim
- Crash
- Ride
- Shaker
- Cowbell
- Tambourine
- Percussion
- FX / One-shot
- Custom
- Unassigned

Drum colors and display order can also be configured.

---

## Playback

Playback modes include:

- Section
- Whole Song
- Selected Bars

Additional options include:

- Loop
- Follow
- Internal clock
- DAW synchronization

The playhead follows the current drum position while active notes and drum rows are highlighted.

---

## Export to Ableton Live

Committed drum patterns can be exported back to Ableton Live as MIDI.

The Export workflow includes:

1. Select the source pattern
2. Select a destination MIDI track
3. Choose an Arrangement position
4. Preview the export plan
5. Write the MIDI data to Live

Existing source OSTF data remains unchanged unless explicitly saved through OSTF editing.

---

## Undo and Editing

Editing tools include:

- Undo
- Redo
- Copy Bar
- Paste Bar
- Duplicate to Next
- Clear Solo / Mute
- Lock protection
- Pattern Bank copy

Locked notes and protected elements are preserved where applicable.

---

## English User Interface

The released version uses an English interface throughout the device.

Japanese and other language data stored inside an OSTF file can still be preserved as song content.

---

## Requirements

- Ableton Live
- Max for Live
- A compatible version of Max included with or supported by your Ableton Live installation

OSTF Drum Arranger is distributed as an `.amxd` Max for Live device.

---

## Installation

1. Download `OSTF_Drum_Arranger_v1.1.amxd`
2. Place the file in your preferred Max for Live device folder
3. Open Ableton Live
4. Drag OSTF Drum Arranger onto a MIDI track
5. Open an OSTF file or create a new song structure
6. Generate, edit, capture, arrange, and export drum patterns

---

## Open Song Timeline Format

OSTF Drum Arranger is built around the **Open Song Timeline Format**.

OSTF is an open format for describing complete song structure and musical information, including sections, harmony, melody, lyrics, arrangement data, timing, and other song-level information.

OSTF Drum Arranger focuses specifically on the drum arrangement workflow while preserving the surrounding OSTF song data.

OSTF 3.5:

https://github.com/yoh-nak/Open-Song-Timeline-Format-3.5

---

## Project Philosophy

OSTF Drum Arranger is not intended to replace a dedicated drum instrument or high-end drum sample library.

Its main purpose is to provide:

- Composition support
- Arrangement support
- Song-structure-aware drum editing
- MIDI capture
- Pattern experimentation
- OSTF integration
- Ableton Live workflow integration

The focus is on **musical workflow and arrangement**, while your preferred Drum Rack, drum instrument, or external sound source handles the final sound.

---

## Version 1.1

Version 1.1 is the corrected public release of OSTF Drum Arranger.

It includes:

- OSTF 3.5 support
- Section-based drum arranging
- Drum pattern generation
- Step editing
- Velocity editing
- Humanize tools
- Fill generation
- Phrase Compare
- Pattern Banks A-H
- Live MIDI Capture
- Drag and Shift multi-selection
- Section assignment
- GM16 mapping
- Drum Rack mapping
- Pad Routing
- MIDI Learn
- Playback feedback
- Section playback
- Whole-song playback
- Export to Ableton Live
- English user interface
- Stable grid rendering
- Improved UI consistency
- Corrected remaining Japanese text in deep editing views
- Corrected visible version labels

---

## Support Development

OSTF Drum Arranger is available for free.

If you find the project useful and would like to support continued development:

**Buy Me a Coffee**

https://buymeacoffee.com/yohsukenak

Your support helps with continued development of OSTF, Max for Live tools, documentation, testing, and future music-production utilities.

---

## Repository

OSTF Drum Arranger for Max for Live

https://github.com/yoh-nak/OSTF-Drum-Arranger-M4L

---

## License

Please refer to the license information included in this repository.

---

## Author

Developed by **yoh-nak**

Open Song Timeline Format / OSTF Max for Live project
