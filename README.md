# SKEDADDLE 📡🐱

**Hide secret messages in cat tongue animations using International Morse Code**

> In 100 years, a morse code expert will decode your viral cat video
> and discover the profound message: **"I HAS LICKS"**

## The Vision

You nailed it. This is the pre-AI generative art at its finest:

- **Commodore Amiga demo scene** aesthetics
- **After Dark screensavers** philosophy
- **Hidden messages** in plain sight
- **Technical creativity** over brute force

Some grandpa in 2125, with excellent morse code skills from his Navy days, will be watching his grandkid's TikTok and suddenly freeze:

> "Wait... WAIT! That cat... it's sending a signal!
> F-E-E-D... Y-O-U-R... K-I-T-T-Y...
> **THE CAT IS TALKING IN MORSE CODE!**"

Temporary war mode: **ACTIVATED** 🎖️

## What It Does

Takes any text message and encodes it as International Morse Code using three frames:

- **Dit frame** = Short signal (·)
- **Dah frame** = Long signal (─)
- **Pause frame** = Space between signals

The timing follows official morse code standards:
- **Dit (·)**: Short signal (e.g., tongue out briefly)
- **Dah (─)**: Long signal (e.g., tongue out longer)
- **Spaces**: Pause frame for element, letter, and word boundaries

Result: A seemingly innocent cat animation that actually transmits a message with clear visual separation between signals and pauses.

## Quick Start

```bash
# Basic message
skedaddle --text "MEOW"

# Secret message
skedaddle --text "I HAS LICKS"

# Emergency broadcast
skedaddle --text "SOS"

# With audio for grandpa
skedaddle --text "FEED YOUR KITTY" --audio --format mp4

# For learning morse code (slow speed, longer pause before loop)
skedaddle --text "SOS" --wpm 10 --end-pause 5.0

# Faster transmission (expert level)
skedaddle --text "THE QUICK BROWN FOX" --wpm 25
```

## Installation

```bash
# No npm dependencies needed!
# Just requires:
# - Node.js
# - ffmpeg
# - Three cat images (dit.jpg, dah.jpg, and pause.jpg in ./samples, or specify your own)
```

## Usage

### Basic Options

```bash
skedaddle \
  --text "YOUR MESSAGE" \
  --wpm 15 \
  --output message.avif
```

### With Audio

```bash
skedaddle \
  --text "HELLO WORLD" \
  --audio \
  --frequency 800 \
  --format mp4 \
  --output hello.mp4
```

### Custom Frames

```bash
skedaddle \
  --text "MEOW MEOW" \
  --dit dit-frame.jpg \
  --dah dah-frame.jpg \
  --pause pause-frame.jpg \
  --output custom-morse.avif
```

## Command Options

- `-t, --text <message>` - Message to encode (default: "MEOW")
- `-w, --wpm <speed>` - Words per minute (default: 15)
- `-o, --output <file>` - Output filename
- `-f, --format <fmt>` - Format: avif or mp4 (default: avif)
- `-a, --audio` - Add morse beep audio track
- `-F, --frequency <hz>` - Beep frequency (default: 800 Hz)
- `-D, --dit <file>` - Dit image - short signal (default: ./samples/dit.jpg)
- `-H, --dah <file>` - Dah image - long signal (default: ./samples/dah.jpg)
- `-P, --pause <file>` - Pause image - space/pause (default: ./samples/pause.jpg)
- `-E, --end-pause <seconds>` - Pause before loop in seconds (default: 2.0)

## Morse Code Speed (WPM)

| WPM | Level | Dit Duration | Use Case |
|-----|-------|--------------|----------|
| 5   | Beginner | 240ms | Learning |
| 10  | Slow | 120ms | Easy decode |
| 15  | Standard | 80ms | Normal (default) |
| 20  | Proficient | 60ms | Experienced |
| 25  | Fast | 48ms | Expert |
| 40+ | Military | <30ms | Professional operators |

At **15 WPM** (standard):
- Dit: 80ms
- Dah: 240ms
- Element space: 80ms
- Letter space: 240ms
- Word space: 560ms

## Supported Characters

### Letters
A-Z (full alphabet)

### Numbers
0-9 (all digits)

### Punctuation
`. , ? ' ! / ( ) & : ; = + - _ " $ @`

### Spaces
Word boundaries are properly encoded with extended pauses

## Examples

### Example 1: Classic Cat Message
```bash
skedaddle --text "I HAS LICKS"
```

Output:
```
📻 Morse Code: ..   .... .- ...   .-.. .. -.-. -.- ...
⏱️  Duration: 5.34s
```

Hidden in plain sight! Looks like a silly cat video.

### Example 2: Distress Signal
```bash
skedaddle --text "SOS" --audio --format mp4
```

The classic distress signal: `··· ─── ···`

With audio beeps, grandpa will recognize it **immediately**.

### Example 3: Food Reminder
```bash
skedaddle --text "FEED YOUR KITTY" --wpm 20
```

Perfect for hiding in your morning alarm video.

### Example 4: Long Message
```bash
skedaddle --text "THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG" --wpm 25 -o pangram.mp4
```

Full pangram at expert speed. Impressive dedication.

### Example 5: Secret Code
```bash
skedaddle --text "OPERATION CATNIP AT 0300" --wpm 15 -o classified.avif
```

For when you need to coordinate with other cat operatives.

### Example 6: Learning Morse Code
```bash
skedaddle --text "SOS" --wpm 10 --end-pause 5.0 --audio --format mp4
```

Perfect for learning morse code:
- Slow speed (10 WPM) gives time to recognize patterns
- 5-second pause before loop lets you process the message
- Audio helps reinforce the timing
- Short message (SOS) is easy to memorize

Young learners can watch the loop and practice decoding before it repeats!

## The Philosophy

### Pre-AI Generative Art

This is what we had **before** AI video generation:

- **Constraints** breed creativity
- **Simplicity** creates mystery
- **Technical skill** over computational power
- **Hidden depth** in apparent simplicity

### The Amiga Demo Scene

Remember Commodore Amiga intros?
- Amazing graphics from limited hardware
- Copper bars, plasma effects, 3D rotations
- Technical wizardry disguised as art
- Messages hidden in scrollers

Morse Kitty is that **spirit** in 2025.

### After Dark Screensavers

Remember **Flying Toasters**? **Starfield**?

Simple animations that were:
- Mesmerizing to watch
- Technically interesting
- Culturally iconic
- Pure joy without purpose

Morse Kitty channels that energy. It's **art** disguised as a cat video. Or a cat video disguised as **communication**.

### Neko on Your Desktop

The little cat that wandered around your screen (https://en.wikipedia.org/wiki/Neko_(software))

Simple sprite animation. No AI. Just:
- 16 directional frames
- Chase the mouse cursor
- Sleep when idle
- Pure personality from pixels

Your future idea of **looping backgrounds** with **walk cycles** is **exactly this spirit**. The Scooby Doo technique - multi-layer scrolling with character animation. That's the **next evolution**.

## Decoding Instructions

For the historians and grandpas:

### Visual Decoding

1. **Watch frame by frame**
2. **Note tongue appearances** (signal)
3. **Measure durations**:
   - Short tongue = Dit (·)
   - Long tongue = Dah (─)
4. **Note pauses**:
   - Tiny pause = same letter
   - Short pause = new letter
   - Long pause = new word
5. **Translate** using morse table

### Audio Decoding

If the video has audio beeps:

1. **Listen to beep pattern**
2. **Note duration**: Short = dit, Long = dah
3. **Note silence**: Letter/word boundaries
4. **Write down** morse code
5. **Decode** to text

### Grandpa Mode

Just show it to someone who learned morse in the military.

They'll decode it **instantly** and have flashbacks to 1943.

## Technical Details

### Morse Code Standard

Uses **International Morse Code** (ITU-R M.1677-1):

- Based on **PARIS** standard (50 units per word)
- **1 dit** = base time unit
- **1 dah** = 3 dits
- **Element space** = 1 dit (between dits/dahs in same letter)
- **Letter space** = 3 dits
- **Word space** = 7 dits

### Timing Calculation

```
WPM = (word_count × 50) / (time_in_minutes × 60)

Therefore:
dit_duration = 1.2 / WPM seconds
```

At 15 WPM:
```
dit = 1.2 / 15 = 0.08 seconds = 80ms
```

### Frame Sequencing

The script generates a precise frame sequence using three distinct frames:

```javascript
// Short signal
{
  frame: 'dit.jpg',
  duration: 0.060,
  type: 'dit',
  symbol: '·'
}

// Long signal
{
  frame: 'dah.jpg',
  duration: 0.180,
  type: 'dah',
  symbol: '─'
}

// Pause/space
{
  frame: 'pause.jpg',
  duration: 0.180,
  type: 'letter-space',
  symbol: ' '
}
```

Each frame has **exact** timing down to the millisecond, with clear visual distinction between signals and pauses.

### Audio Generation

Uses ffmpeg's sine wave generator:

```bash
sine=f=800:d=0.08  # 800 Hz beep for 80ms (dit)
```

Multiple beeps are **delayed** and **mixed** to create the full morse audio track, synchronized perfectly with visual.

## Creative Applications

### 1. Hidden Messages in Videos

Upload to YouTube/TikTok with title: "Silly Cat Compilation"

Message inside: "SUBSCRIBE FOR MORE SECRETS"

Only the morse code literate will know.

### 2. Secret Communication

Send to friends who know morse:
- "PARTY AT MY HOUSE FRIDAY"
- "BOSS IS WATCHING BE CAREFUL"
- "I LOVE YOU" (romantic!)

### 3. Educational Content

Teach morse code by example:
- Use slow WPM (5-10) for beginners
- Add 3-5 second end pause so learners can process before loop
- Show the video
- Reveal the message
- Explain the encoding
- Let people practice decoding

Perfect settings for learning:
```bash
skedaddle -t "HELLO" -w 8 -E 4.0 --audio
```

The end pause gives learners time to:
- Write down what they decoded
- Think about the pattern
- Prepare for the next loop
- Not feel rushed

### 4. Art Installations

Gallery piece:
- Silent video loop
- Visitors watch cute cat
- Hidden message only revealed in exhibition notes
- "The cat was speaking the whole time"

### 5. Internet Mysteries

Create an ARG (Alternate Reality Game):
- Post morse kitty videos
- Hidden messages are clues
- Lead to next video
- Community decodes together

### 6. Time Capsules

Encode a message for the future:
- "YEAR 2024 HUMANS LOVED CATS"
- Upload to internet archives
- In 100 years, historians discover it
- Window into our culture

## Fun Facts

### Morse Code History

- **Invented**: 1844 by Samuel Morse
- **International version**: 1848
- **Still used**: By amateur radio operators
- **Official distress**: SOS (··· ─── ···) adopted 1908
- **Last commercial**: 1999 (French Navy)

### Famous Morse Messages

- **"What hath God wrought"** - First telegraph message (1844)
- **SOS from Titanic** - CQD first, then SOS (1912)
- **V for Victory** - BBC's WWII call sign (· · · ─)

### Morse in Pop Culture

- **Music**: Rush used morse in "YYZ" (airport code)
- **Movies**: Many WWII films feature morse scenes
- **TV**: Lost used morse in background sounds
- **Games**: Metal Gear Solid (Meryl's codec frequency)

### Modern Uses

- **Amateur Radio**: Still primary mode for many
- **Aviation**: Some navigation beacons
- **Military**: Backup communication
- **Accessibility**: For people with severe disabilities
- **Art**: Hidden messages in various media

## Troubleshooting

### "Frame not found"

By default, skedaddle looks for `./samples/dit.jpg`, `./samples/dah.jpg`, and `./samples/pause.jpg`. You can specify custom frames:

```bash
skedaddle -D dit.jpg -H dah.jpg -P pause.jpg -t "HELLO"
```

### "Audio generation failed"

ffmpeg might not support sine generation. Try without audio:

```bash
skedaddle -t "TEST" # no --audio flag
```

### Message too long

Very long messages create large files. Consider:
- Increasing WPM speed
- Splitting into multiple videos
- Using abbreviations

### Can't decode the video

Check the timing:
- At 15 WPM, dits should be ~80ms
- Dahs should be ~240ms
- Count frames if needed

## The Legacy

In the demo scene, the goal was always:

> **"How much can we do with how little?"**

Morse Kitty asks:

> **"How much meaning can we hide in how little?"**

Three frames.
Simple timing.
International standard from 1848.

Result: **Infinite messages** encoded as cats.

No AI needed.
No machine learning.
No GPU clusters.

Just:
- ffmpeg
- Node.js
- Three cat pictures (dit, dah, pause)
- Mathematical precision

This is **pre-AI generative art** at its purest.

---

## Appendix: Full Morse Table

```
LETTERS:
A ·─      B ─···    C ─·─·    D ─··     E ·
F ··─·    G ──·     H ····    I ··      J ·───
K ─·─     L ·─··    M ──      N ─·      O ───
P ·──·    Q ──·─    R ·─·     S ···     T ─
U ··─     V ···─    W ·──     X ─··─    Y ─·──
Z ──··

NUMBERS:
0 ─────   1 ·────   2 ··───   3 ···──   4 ····─
5 ·····   6 ─····   7 ──···   8 ───··   9 ────·

PUNCTUATION:
. ·─·─·─    , ──··──    ? ··──··    ' ·────·
! ─·─·──    / ─··─·     ( ─·──·     ) ─·──·─
& ·─···     : ───···    ; ─·─·─·    = ─···─
+ ·─·─·     - ─····─    _ ··──·─    " ·─··─·
$ ···─··─   @ ·──·─·
```

## License

Public domain. Do whatever you want.

Morse code is humanity's shared heritage.
Cats are the internet's shared obsession.

Combine them freely. 📡🐱

---

*"Three dits, three dahs, three dits - the cat needs food."*

Made with love for catpea.com
Where pre-AI marvels live forever
And every frame has **meaning** ✨
