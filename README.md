# Jukebox-Ai-music-prompt-Generator
Suno tool for making ai music using claude, chatgpt, or any ai platform
MULTI-GENRE FULL UNIVERSE ENGINE
AI Lyric Prompt Generator
Built from 3,000+ songs. One click. Endless output.

What Is This?
The Multi-Genre Full Universe Engine is a prompt generator that produces AI-ready lyric briefs at the click of a button — combining a lyric scenario, a song structure, a vocal style, and a soundscape into a single ready-to-paste prompt for any AI writing tool (Claude, ChatGPT, Gemini) or music generation platform (Suno, Riffusion).
Every output is guaranteed to land within one person's actual musical taste — because the entire engine was built from the ground up using their real listening library.

The Numbers
The engine draws from four independent pools, combined randomly on every generation:
PoolCountLyric scenario prompts107Song structure arcs18Soundscape profiles84Vocal style profiles85
107 × 18 × 84 × 85 = 13,758,840 unique configurations
Each vocal profile also embeds three distinct delivery variants (ballad / uptempo / arena), pushing the effective mechanical number to approximately 41 million distinct outputs before the AI model is even involved.
Add in that no AI model produces the same lyrics twice from the same prompt, and that conversation history and memory drift the model's style over time, and the practical output space is effectively endless.

How It Was Built
This is not a tool built from assumptions about what good music sounds like. It was reverse-engineered from a real listening library using a multi-step data pipeline:

Extract the library. A custom Python script scanned a 3,000+ song music library and extracted all filenames.
Clean and separate. The raw filename list was fed to an AI model to remove duplicates, strip song titles, and isolate artist names into a clean list.
Manual pruning. Artists that belonged to other household members or weren't personally listened to were removed by hand. What remained is a genuine personal taste profile.
Generate lyric scenarios. Song titles from the library were fed to an AI model in batches to extract thematic and emotional lyric prompts — capturing the kinds of stories and feelings that actually resonate.
Build vocal and sound profiles. Artist names were converted in batches into detailed vocal style descriptors and genre-appropriate soundscape profiles through iterative prompting and refinement.
Trial and error refinement. The prompt format was tested against multiple AI tools and music generators, refined until the outputs consistently sounded right — the kind of music the library actually represents.


How to Use It
For AI Lyric Writing (Claude, ChatGPT, Gemini)

Click ENTRAINMENT to copy the style guide to your clipboard.
Paste it into a new AI conversation to set the context.
Click GENERATE ALL NEW to produce a fresh combination.
Copy the FULL PROMPT and paste it as your next message. The AI will write lyrics in the selected style.
Lock any section you want to keep and regenerate the rest for endless variation.

For Music Generation (Suno, Riffusion)
Use the MUSIC PROMPT output — this version has artist names automatically removed to comply with platform guidelines, while retaining the full vocal and sonic description.

Controls

GENERATE ALL NEW — randomizes all four unlocked sections simultaneously.
MUTATE — re-rolls a single section while leaving the others in place.
LOCK / UNLOCK — freezes a section so it survives the next generate.
ENTRAINMENT — copies the full style guide to the clipboard for pasting into an AI conversation.
FULL PROMPT — the complete prompt for AI lyric writing, including artist context.
MUSIC PROMPT — the Suno/Riffusion-safe version with artist names stripped.
A− / A+ — adjusts the text size in the interface.


What Each Output Contains
Lyric Scenario
A thematic or emotional writing brief — the subject matter, perspective, and emotional arc of the song. Drawn from the moods and themes present in the source library.
Structure Arc
The architectural shape of the song — how it builds, breaks, repeats, or resolves. Includes optional delivery cues like whispered, screamed, or half-rapped passages.
Vocal Style
A detailed description of how the vocals should sound — timbre, placement, delivery dynamics, genre character, and three embedded delivery variants (ballad, uptempo, arena). Artist-tagged in the full prompt; scrubbed for music platforms.
Soundscape
The instrumental and sonic context — instrumentation, texture, energy level, and how the mix should support the vocal. Fully platform-safe, no artist references.

Requirements

Python 3.x
tkinter (included in standard Python on Windows)
pyperclip — install via pip install pyperclip
