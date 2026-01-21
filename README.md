# Wisteria Motif's FL Studio Piano Roll Scrips
A collection of my python scrips for the FL Studio Piano Roll.   
*(Well, for now there is only one script, but who knows.)*

## Advanced Velocity Fades
[Link to FL Studio Forum post.](https://forum.image-line.com/viewtopic.php?t=311614)
![Advanced Velocity Fades preview image](https://github.com/WisteriaMotif/FL_Studio_Piano_Roll_Scripts/assets/143191748/d9076409-efb6-40c7-8eb1-8c1b2ed96f4b)

- Velocity L/R: The velocity of the leftmost/rightmost note(s).
- Dynamic: The overall dynamic of the notes. The default value is 1. Values over 1 will increase the dynamic.
- Dynamic Pinch: Reduces the dynamic towards the outmost notes. Values below 0 will pinch towards the left, while values over 0 will pinch towards the right.
- Curve: Adds a curve to the fade.
- Zero Velocity Protection: Stops notes' velocity from becoming 0. Helpful for instruments that simply don't play notes when the velocity is 0, yet you still want the notes audible.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Updated Screenshot (MIDI 0-127 Dialog)

![Updated Velocity Dialog](images/advanced-velocity-dialog.png)

Or full size preview:
![Large Preview](https://github.com/Camburgerhelpers/Advanced-Velocity-Fades-MIDI/raw/main/images/advanced-velocity-dialog.png)

## MIDI 0–127 Edition (Fork by Camburgerhelpers)

This is a tweaked version of the original **Advanced Velocity Fades** script, focused on MIDI workflows.

### Key Changes
- Velocity L/R inputs now use **integer 0–127 MIDI values** (via `addInputKnobInt`) instead of 0.0–1.0 floats/decimals  
  → Knobs snap to whole numbers — no manual conversion or calculator required
- Initial L/R values are auto-converted from selected notes and rounded to the nearest MIDI value
- Zero-velocity protection defaults to enabled (~MIDI 1 minimum to avoid silent notes)
- All original features (Dynamic, Dynamic Pinch, Curve, etc.) remain unchanged

### Installation (for this fork)
1. Download the file: `Advanced Velocity Fades MIDI 127.pyscript` (from this repo)
2. Place it in:  
   `Documents\Image-Line\FL Studio\Settings\Piano roll scripts\`
3. Restart FL Studio or reload the Piano Roll
4. Select notes in time order → run from the Scripts menu
5. Enter Velocity L/R directly as 0–127 integers

Tested in FL Studio 2025.

**Original author:** Wisteria Motif  
**Original repo:** https://github.com/WisteriaMotif/FL_Studio_Piano_Roll_Scripts  
**Original forum post:** https://forum.image-line.com/viewtopic.php?t=311614

Feel free to fork or contribute further!
