---
title: "What is lossless?"
date: 2026-03-22
categories: [Audio]
tags: [lossless, lossy]
math: true
---

# Lossless Music

##### 	***Lossless and lossy are defined strictly relative to the source, not by some arbitrary frequency cut-off or bitrate threshold.***

> Define Lossless Here

> Define Lossy Here

---

#### What the hell is a source?

You could find a hundred different definitions for a "source file" if you really want to over-complicate things. Some will argue it’s the raw mix right before dithering and mastering effects are applied. Others will go full purist and claim the original analog multi-track tapes are the only true source. In my book, however, the source file is simply the final, definitive master leaving the studio when production wraps heading for the pressing. The bitter reality is that you do not, cannot, and will not ever own this file, unless you decide to break into the record label's archive. Because we can't have the actual master, we take the closest verifiable thing we can get our hands on and declare *that* our source. This is where things get spicy.

In the archiving world, your source usually comes from one of two main mediums: physical media rips (CD, Blu-ray, Vinyl, SACD) or, thanks to the internet, digital files sourced from streaming platforms (Apple Music, Tidal, Qobuz, Deezer) and digital storefronts (Bandcamp, HDtracks) - collectively referred to as WEB. All of them are also categorized as Analog and Digital Mediums.

**Analog Physical Mediums:** Vinyl and Cassette tapes are the oldest form of music distribution; they are fundamentally analog. Vinyl stores the soundwave of your favorite album as a physical shape; literally cutting grooves in the vinyl disc. A needle traces those grooves and a cartridge translates the vibrations into electrical signals (analog), which pass through a phono preamp for correction and amplification, then into an amplifier, and finally to your speakers. To capture that signal digitally instead, an ADC intercepts it after the preamp to sample it into snapshots. The lossless/lossy framework doesn't cleanly apply here although lossless-ness of a vinyl disc can be judged by the condition of the disc (i.e. how many times it was played, what's the state of the disc after the plays, quality of the equipment used on it). The characteristics of a vinyl (like warmth, surface noise, dynamic range, impact on loudness war) and the debates around it are very interesting. More on that some other day. Moving on to Cassettes, a tape recorder alters the magnetization of magnetic tape in a cassette tape to record the soundwave. Unless it is the only source of a certain record, nobody really cares about cassettes anymore. They aren't 'lossy' in the digital sense, but they suffer from severe analog degradation, tape hiss, and physical generation loss every time you play them. A nightmare for preservation.

**Digital Physical Mediums:** Step out of analog and into digital, and sound stops being a physical shape. It becomes numbers. But before the numbers themselves, the hardware that stores them. A CD stores audio as a spiral of microscopic pits and lands pressed into a polycarbonate disc. A laser reads that spiral, interpreting each pit and land as a binary value. String enough of those values together and you have PCM audio data. A standard disc holds up to 74–80 minutes of audio at 16-bit/44.1kHz. CD is the standard source for digital archival for two reasons: it is the most common and accessible distribution format - sometimes the only format a release ever sees - and it has CIRC: a system that mathematically reconstructs the exact, bit-perfect original audio data from scratched or damaged sections of the disc. Then came the formats that tried to push beyond CD's ceiling. SACD and DVD-Audio both arrived at the same time, taking opposite approaches. SACD abandoned PCM entirely and used DSD. DVD-Audio stuck with PCM but stretched it to 24-bit/192kHz. Right idea, wrong decade - both, and honestly the entire physical distribution medium, had to lose to the MP3. Blu-ray arrived later as a video format that happened to support hi-res lossless audio as part of its spec. Some labels have been using it to distribute hi-res surround and stereo mixes.

**WEB:** Digital files sourced from streaming platforms (Apple Music, Tidal, Qobuz, Deezer) and digital storefronts (Bandcamp, HDtracks) are collectively referred to as WEB. The convenience these platforms have brought is undeniable; we are getting files directly from the distributors themselves. No hassle of disc conditions or pressing quality. But they are not saints. Take the album *Wish You Were Here* by Pink Floyd. The original 1975 release was remastered in 1994. Then in 2011, James Guthrie remastered it again and delivered a brand new stereo remix alongside a 5.1 surround mix. Then it got remastered once more in 2016. Four distinct versions of the same album across five decades. Log onto any major streaming platform today and you will find only one of them sitting there with no indication of which one it actually is. We have no idea if we're listening to the original mix or a remix or a remaster! Some will argue it is not sensible to host all four versions simultaneously. I would argue the opposite; hosting these pieces of history is any day more important than storing millions of AI slops on the same servers. That leads us to the authenticity, the *Hi-Res FLAC or ALAC* files on the platforms, are they truly what they claim to be? It might be rare for western distributors, but it's very common to find a 16-18 kHz hard cut-off file labelled as *16-bit, 44.1 kHz* or even worse, *24-bit, 48/96/192 kHz* in Indian releases.

So what do these bits, kHz actually mean? Enter Sample Rate, Bit Depth, Bitrate. Let's establish the units.

---

#### Units & Measurements

Picture a water wheel - actually, not one but an entire mill. Think of the water flowing through as the sound wave the computer is trying to capture. The size of each bucket - how much water it can hold - that's Bit Depth. How many buckets each wheel scoops per second, that's Sample Rate. And the number of wheels is your channels - one wheel for mono, two for stereo, six and eight for multi-channel music.  And the total water delivered per second across each channels combined, which is just those three multiplied together, that's Bitrate. The bigger the buckets, the more frequently they scoop, the more faithfully the wheel captures the stream.

**Frequency** 
The number of times a wave of sound completes a full cycle per second is its frequency, measured in Hertz (Hz). A slower wave results in a lower frequency, while a faster wave creates a higher frequency. You may wanna look at this table - might come in handy while looking at a spectrogram:

| Range     | Frequency    | What Lives Here              |
| --------- | ------------ | ---------------------------- |
| Sub-bass  | 20–60 Hz     | Rumble, felt more than heard |
| Bass      | 60–250 Hz    | Kick drums, bass guitars     |
| Low-mid   | 250–500 Hz   | Warmth, muddiness            |
| Midrange  | 500 Hz–2 kHz | Vocals, guitars, keyboards   |
| Upper-mid | 2–6 kHz      | Presence, attack, clarity    |
| Treble    | 6–20 kHz     | Cymbals, hi-hats, air        |

By the way, sound below the human hearing threshold (20 Hz) is classified as infrasound, and sound above it (20 kHz) is ultrasound. 

**Sample Rate** 
While frequency describes how fast a sound wave moves in the air, sample rate (also measured in Hertz) is the speed at which a computer takes "snapshots" of that wave at regular intervals to turn it into digital data. 

Nyquist-Shannon sampling theorem says that to accurately reconstruct a continuous sound wave from those audio snapshots, your sample rate must be at least twice the highest frequency you want to capture. Going below that threshold will introduce aliasing - the wave folds back on itself and produces completely false frequencies that weren't in the original signal. If we want to capture as much as human ears can hear - that is 20 kHz, we have to double the sample rate to accurately capture the sound, at 40 kHz. That is why CD quality (44.1 kHz) is a standard; we get 4.1 extra kHz of sample rate that gives us a little breathing room - although the existence of those extra kilohertz in a CD is just a historical coincidence.

Earlier when we talked about Analog sound and Vinyl, I mentioned Analog-to-Digital Converter (ADC). When you "rip" a vinyl, you can set the ADC to capture at 24-bit/192kHz (you may have also seen some rips at 32-bit/384kHz or even at DSD64 to all the way up to DSD256). And it will absolutely fill that container. But what is it actually capturing? Most of the musical elements (vocals, instruments) naturally roll-off around 16-18 kHz. Everything above that is stylus noise, surface resonance, and ultrasonic cartridge artifacts. Technically real data from the vinyl, but not music.
Which raises another question, if your entire music is done by 18kHz, then what's the point of 48kHz, 96kHz or 192kHz? The point is headroom. Any mathematical artifacts that get generated by effects processing during the mixing (EQ curves, reverb tails, pitch correction, etc.) get pushed so far above the audible range that they're completely inaudible by the time the mix is rendered down to 44.1kHz. So aren't those extra sample rates unnecessary for me and shouldn't they be just stripped away after the production is complete? The answer is the moment you apply any kind of filter to remove content above any certain frequency - even the most mathematically perfect low-pass filter introduces phase artifacts at the edges of the cut - you've touched the signal and the cleanest thing you can do to a signal is to leave it untouched.

**Bit Depth & Dynamic Range**

When a computer takes a snapshot of a sound wave, it needs to store the height of the wave at that exact moment - the amplitude. But computers can't store infinite precision. They have to round the amplitude to the nearest available value. The tiny difference between the real value and the stored value becomes an error that accumulates across the whole recording. The rounding errors are called quantization noise. At low bit depths this is audible as distortion. At 16-bit it's below perception. At 24-bit it's essentially theoretical.

<details> <summary> Cool to know</summary>
A 1-bit system has only 2 possible values. On or off. The wave is either at maximum or at zero. Those 80s-90s crunchy video game sounds are an example of a 8-bit system that has 256 possible values. The wave exists but it's a rough approximation. The CD quality or a 16-bit system has 65,536 possible values. The rounding errors in this system are imperceptible to human ears under regular listening conditions. The rounding errors for a 24-bit system (16,777,216 possible values) are so small; they're buried beneath the noise floor of any real world listening environment.</details>
Every system has a floor and a ceiling. The ceiling is the maximum amplitude the system can store without distorting. Pushing past it introduces clipping - where the top of the sound wave gets chopped off. The floor is more interesting. It's not silence. It's the point where the audio signal becomes indistinguishable from the noise the system itself generates just by existing: hissing. When the music gets quiet enough to fall below that noise floor and disappears into it you hear hiss.
Dynamic range is the gap between those two points. How much distance exists between the noise floor and the clipping ceiling. Measured in decibels. Now here's where bit depth connects directly. Every bit you add to the system roughly doubles the number of amplitude values available, which pushes the noise floor down by about 6dB. More values means finer gradations means quieter quiets before the signal dissolves into noise. 16-bit gives you 96dB of dynamic range. 24-bit gives you 144dB. 16-bit covers most real world listening comfortably. 96dB covers everything from the quietest audible sound to a live concert. The extra headroom found in 24-bit matters most during recording and mixing; engineers need room to work without accidentally clipping any data.
The rip of the very first and highly sophisticated Japanese CD pressing (The Black Triangle) for the album *The Dark Side Of The Moon*, which is 16-bit has more dynamic range than the 24-bit Vinyl rip of the "2011 Discovery Remaster". To answer why, let's shortly address the sneaky elephant in the room before finishing: Loudness War.
One more thing, Dynamic Range is measured as a single number - DR score. How the math is calculated is irrelevant for today. DR13 means a wide, dynamic recording. DR5 means it's been squashed flat. The scale runs roughly from DR1 (a brick wall) to DR20+ (orchestral recordings with extreme quiet-to-loud swings). Most modern pop and rock masters land somewhere between DR5 and DR9 (gratitude to the elephant in the room). For most cases, files above DR11-12 can be considered gold.

**Bitrate** 
Remember those water wheels? Mathematically, bitrate is nothing but a simple product of these three variables: $Bit\ Depth\times Sample\ Rate\times Channels$. For compressed lossless formats like FLAC, bitrate varies depending on the complexity of the music. However, for a special case, bitrate is constant! The bitrate for a CD rip file in an uncompressed PCM format (a `.wav` file for instance) is always 1411 kbps. Let's see the math.
A standard CD-quality file has:
Bit Depth: 16-bit, Sample Rate: 44.1 kHz or 44100 Hz, Channels: 2. 

So the bitrate for a CD rip is = $$ 44,100 \times 16 \times 2 = 1,411,200 \text{ bits per second or 1,411 kbps} $$

Pink Floyd's Jug Band Blues is exactly 3 minutes long. To capture this song in those exact settings, 1,411 kilobits data were transferred every second for 180 seconds. So, the total amount of data transferred was:
						$\text{Bitrate} \times \text{Duration (seconds)} = \text{Total Bits}$
						$1,411,200 \text{ bps} \times 180 \text{ s} = 254,016,000 \text{ bits}$
												 $\approx 3.75\ \text{MiB}$
You may not see the exact number in your own file because we did not take milliseconds, metadata tags and the file container's own metadata into account.

If someone hands you a file claiming it's a 24/192 Vinyl rip, all you have to do is convert the file to an uncompressed lossless format (if not already) and compare it against the math. If you see the values are not similar, then congratulations, you've found an upscale! The math doesn't lie, but now you know who did.

We got the units right. What to do with this information now? Enter Sandman.

---

#### Codecs & Containers

---

**Codec vs Container**
A codec is the algorithm - the set of formulas to encode and decode audio data. A container is the file format that wraps the encoded audio, along with metadata like track title, album art, and replay gain. They are not the same, and conflating them is a reliable way to confuse yourself. A `.wav` file is a container holding uncompressed PCM. A `.flac` file is a container holding FLAC-encoded audio. The codec handles what happens to the numbers; the container handles where they live.
Codecs are either Lossless or Lossy. And one of the culprits behind this authenticity war.

**Lossless codecs** make bit-perfect identical copy of the source file and use different algorithms to store it. If your source file is already lossy, the codecs will make a lossless copy of *that* source file. You have essentially changed the vessel of your already damaged file without further damage. However, relative to *that source file*, your new one is lossless. Lossless codecs can be separated into Uncompressed and Compressed.
Practically, this is what both of these are:
![Cooler Daniel](/assets/posts/what-is-lossless/danielvscoolderdaniel.jpg)

---

<u>Uncompressed Lossless</u>

**PCM & DSD**

The sound wave is continuous. It exists at every point in time with infinite possible heights. Computer cannot store all that. So **PCM** says: pick a moment, measure the height(amplitude), write that number down. Wait an identical amount of time. Pick the next moment, measure, write it down. Repeat forever. That's it. Pulse - Code - Modulation. You're pulsing (sampling at regular intervals), coding (converting the height into a number), and modulating (the numbers represent the changing wave).
The output is literally just: `4, 7, 12, 19, 24, 27, 26, 21, 13, 5, -4, -13...`
That list of numbers is the audio. The wave itself, expressed as a sequence of amplitude values over time. Your DAC on playback reads that list from left to right, converts each number back into a voltage, sends it to your speakers, and the speaker cone moves accordingly - the sound is reconstructed.
Sample rate decides how often you're measuring. And just like a camera, more the frame rate, smoother the video. Bit depth decides how precisely you can express each measurement. 16-bit gives you 65,536 rungs on the ladder. 24-bit gives you 16,777,216.

WAV(`.wav`) & AIFF(`.aiff`) are containers that store the raw PCM numbers exactly as they're without any further processing or encoding and then wraps them with metadata tags. The bitrate of a WAV/AIFF at a certain setting is constant. So a CD-quality WAV file runs around 10 MB per minute. For a 74-minute album, that's roughly 740 MB. That is the drawback of these: enormous file size. To shrink this enormity and inefficiency, compression algorithms were invented.

Where PCM measures amplitude at regular intervals using multiple bits, **DSD** flips the approach entirely. It samples only in a 1-bit environment, but at a staggering 2.8224 MHz (64 times the CD sample rate). Instead of asking "how high is the wave right now?" it asks "is the wave going up or down" 2.8 million times per second. An elegant alternative to PCM on paper. However, in practice, DSD is a nightmare for the mixing. Remember why mixing engineers work at 24-bit: that 144dB of dynamic range means *processing artifacts* never get close to anything audible. DSD64 offers around 120dB. But this is *headroom for playback*, what mixing demands is *processing headroom*; How much room exists for arithmetic errors to accumulate without surfacing. And that's determined by how many amplitude values you have available, not how wide the gap between floor and ceiling is.
When you apply any processing during a mix, you're performing mathematical operations on the audio data. The rounding errors generated during operations fall between the available amplitude rungs. At 24-bit PCM you have 16,777,216 rungs on the ladder. Those errors are so small they're buried decibels below anything a human ear could ever detect, even after hundreds of processing passes. At 1-bit DSD, you have only 2 rungs. Up or down. Every mathematical operation that produces a value between those two states has nowhere to land. The errors will be enormous relative to the signal. The processing artifacts don't disappear into the noise floor, they accumulate audibly in the signal itself.

<details> <summary>The workaround studios landed on is DXD.</summary>
    Digital eXtreme Definition, which is literally just very high-resolution PCM at 24-bit/352.8 kHz. Raw DSD gets converted to DXD, all the mixing and mastering happens there, then it gets converted back to DSD for release. For older catalog titles the chain was simpler: analog master tape → PCM workstation → DSD. To conclude, for the vast majority of releases, a DSD file touched PCM at some point during production. Native end-to-end DSD productions are genuinely rare.</details>

DSF(`.dsf`) and DFF(`.dff`) are the two containers for DSD. They're not equivalent though. DFF stores raw DSD data with no compression and has poor metadata support. DSF applies a mild lossless compression to the DSD bitstream and handles metadata tags properly. In practice, DSF is the preferred archival container for DSD for both reasons.

PCM is the dominant underlying technology behind all of the audio you hear digitally. Every audio file decodes back to PCM when the DAC converts it to sound (except true 1-bit DACs, that work natively with DSD). 

> So, PCM and DSD are also codecs? 
> Yes and no. PCM and DSD are encoding *schemes* - they define how analog sound gets represented as digital data. But they're not codecs in the practical sense people mean when they say codec. A codec is specifically the algorithm that compresses and decompresses already-digitized audio. PCM is what's *inside* the container before any codec touches it. FLAC is a codec because it takes raw PCM and compresses it. 



---

<u>Compressed Lossless</u>
We know that PCM is just a list of numbers. `[100, 102, 101, 103, 102...]`. Each number is the amplitude of the wave at a specific moment. The trick compression algorithms do is that audio data is not random. It's continuous, predictable, structured. If the value at moment `A` is `100`, the value at moment `A+1` is almost certainly going to be close to `100`. It's not going to jump to `5000` unless there's a massive transient. This predictability is the loophole these algorithms exploits. There's always skepticism when you tell someone a file is both "smaller" and "identical." It sounds like a contradiction. If MP3 shrinks files by deleting data, what did FLAC delete to save space? Nothing (although technically it deletes the entire source PCM file).
Most common Compressed Lossless codecs are FLAC (`.flac`), ALAC (`.alac`), APE (`.ape`), WavPack (`.wv`) etc. Let's talk about FLAC.

---

How **FLAC** does what it does?

Step 1: Divide and Conquer (Frames)
FLAC doesn't try to swallow the whole song in one go. It breaks the audio into tiny blocks called frames. Typically, each frame contains 4096 audio samples (sometimes it varies depending on the file).
Why? Because music changes. The predictability of a snare hit is different from a violin sustain. By breaking the stream into blocks, FLAC can adapt its math every few milliseconds to match exactly what's happening in that specific moment. It's like breaking a complex molecule into atoms; once you're looking at the simplest pieces, the rules become obvious.

Step 2: The Prediction Game
Here's the core trick. Instead of storing the actual sample values, FLAC tries to guess them based on the previous ones. It uses something called Linear Predictive Coding (LPC). In plain English: it looks at the past to predict the future.
$$
\text{Next Sample} \approx (a_1 \cdot \text{Previous}_1) + (a_2 \cdot \text{Previous}_2) + (a_3 \cdot \text{Previous}_3) + \dots
$$
Those $a_n$ values are coefficients. Think of them as "confidence levels."
*   Coefficient 0.9: "I trust the last sample a lot."
*   Coefficient 0.1: "The sample before that barely matters."

FLAC tests different orders of prediction (up to 32 previous samples) to find the one that fits the current frame best.

Step 3: Storing the Error
Since the prediction is rarely perfect, there's a difference between the Guess and the Reality. This difference is called the Residual.
$$
\text{Residual} = \text{Actual} - \text{Predicted}
$$
Example:

```
Actual:     [100, 102, 101, 103]
Predicted:  [100, 100, 102, 101]
Residual:   [  0,  +2,  -1,  +2]
```
Step 4: Packing the Residuals and Redundancies
Now that we have a list of tiny numbers centered around zero, we compress them.

- Rice Coding: This is the main engine. It assigns fewer bits to small numbers (which happen often) and more bits to large numbers (which are rare). It's like Morse code: common letters get short dots, rare letters get long dashes.
- Run-Length Encoding (RLE): This is the shortcut for silence. If you have 1,000 samples of absolute silence (zeros), FLAC doesn't write "0" 1,000 times. It writes "0 × 1000". This handles long pauses, dead air, or repeated patterns with almost zero overhead.

Step 5: Stereo Decorrelation
For each frame in stereo audio, FLAC stores the channels in 2 methods:

1.  Independent Mode: FLAC stores $L$ and $R$ separately.
2.  Mid-Side Mode: FLAC calculates:
    *   Mid: $\frac{L + R}{2}$ (The average/center info)
    *   Side: $L - R$ (The difference/stereo info)

For most efficiency, FLAC uses the second one. If the song is mono (L = R), the *Side* becomes all zeros. Zero compresses incredibly well (often down to nothing). Most vocals, kicks, and snares are centered (L ≈ R). The *Side* channel will contain very small numbers (close to zero), which Rice Coding compresses efficiently. If L and R are very different, the *Side* numbers get larger. If they get too large, FLAC switches back to *Independent* mode for that frame. It's adaptive.

Finally, a FLAC file stores:

- Metadata Tags
- Prediction Formula
- Coefficients
- Compressed Residuals

It stores the recipe to reproduce the sound wave. The decoder (your CPU) takes these ingredients, reverses the math ($\text{Actual} = \text{Formula} + \text{Residual}$), and spits out bit-perfect PCM. No approximation.



**ALAC** (Apple Lossless Audio Codec) works by using a similar "predict and record the difference" method, but it is specifically *optimized* for Apple's hardware ecosystem (lmao) and wrapped in an `.m4a` container. The output is mathematically identical to FLAC. But FLAC wins on efficiency.

- Prediction: FLAC supports a higher prediction order (up to 32), meaning it can look further back in the audio to make a tighter guess. ALAC is optimized for decoding speed on Apple chips, which means it sometimes sacrifices compression ratio for battery life.
- Blocking: FLAC uses *variable block sizes* (It can shrink the frame to ~1100 samples for a complex snare hit, or expand to 4096 for a violin sustain). ALAC typically uses *fixed block sizes* (usually 4096). It's less adaptive, which is why ALAC files are often slightly larger than their FLAC counterparts.

To the ALAC glazers: Remember to zip up Steve's when you're done.

---

**Lossy Codecs**

<details> <summary>Think of it like image files.</summary> Take a raw photograph straight off a camera sensor — massive file, every pixel at full precision. Now save it as a JPEG. The algorithm looks at regions of similar color and says: these 40 pixels are all slightly different shades of blue, but nobody will notice if I store them as one shade. Gone. When you zoom in close enough you see the blocks, the smearing, the artifacting. At normal viewing distance you see a photo. But that's what lossy is. Replacing precision with a calculated approximation, banking on the limits of human perception to cover the difference.


YET TO WRITE



> ***Like the dust on a butterfly's wing; to touch it is to erase it.***



<details><summary>What about MQA?</summary> MQA (Master Quality Authenticated) was a proprietary lossy format that claimed to be lossless and charged licensing fees to both hardware and software companies to decode it. It was a solution looking for a problem. Multiple independent measurements confirmed it introduced audible distortion and discarded data. Everyone has moved on; FLAC won, again.</details>			

---

#### Spectrograms

---

#### Metadata Forensics

---



