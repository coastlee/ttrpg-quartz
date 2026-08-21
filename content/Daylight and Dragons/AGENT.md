# Initial Concept

## Map of Concepts (MOCs)

I want to use Codex in this directory to easily generate markdown notes in the "Map of Concepts (MOCs)" style. The idea is that notes will be linked to maps, which will accessible from the directory's home note and easy navigate around. I want Codex to be able to categorize and tag notes and provide other recommendations for how to link notes together.

## Directory's Purpose

This directory is for capturing game notes from live tabletop roleplaying game sessions. I take notes by hand in person and then dump the handwritten notes into this directory. I want Codex to be able to pick up on things like Locations, NPCs, items, other characters, etc and generate individual notes for each instance of a character, location, or item. Help me generate an intuitive MOC structure based on the intended purpose of this project. I want to capture the lore of the world (I'm a player within it), characters, sessions, threads our characters are pursuing, NPCs, and so forth.

## Partylog

Review @partylog.md for instructions on how to use partylog, which is a format for logging game sessions. My handwritten notes attempted to capture the partylog style, but I want Codex to able to pick up on that format and provide recommendations on how to tweak my deposited note to more accurately reflect the partylog style.

## Raw Notes

My raw notes are handwritten notes that I take in person during game sessions. They live in the @raw_notes directory. I want Codex to detect if it's already parsed one of these notes by referencing @raw_notes/parsed.csv. If not, prompt me to parse it. Once parsed, update @raw_notes/parsed.csv with the new entry.

Output the parsed note to @parsed_notes/ with the session date. Wikilink `[[note link]]` items that are mentioned in the note to other notes. Extract any relevant information from the parsed note and store it in the appropriate linked note. Create new notes for any items that are not already linked and populate them with the information found in the parsed note.
