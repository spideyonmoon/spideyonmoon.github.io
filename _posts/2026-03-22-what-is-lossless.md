---
title: "What is lossless?"
date: 2026-03-22
categories: [Audio]
tags: [lossless, lossy, audiophile]
math: true
---
# Lossless Music

##### ***Lossless and lossy are defined strictly relative to the source, not by some arbitrary frequency cut-off or bitrate threshold.***

> Define Lossless

> Define Lossy

---

#### What the hell is a source?

You could find a hundred different definitions for a "source file" if you really want to over-complicate things. Some will argue it’s the raw mix right before dithering and mastering effects are applied. Others will go full purist and claim the original analog multi-track tapes are the only true source. In my book, however, the source file is simply the final, definitive master leaving the studio when production wraps heading for the pressing. The bitter reality is that you do not, cannot, and will not ever own this file, unless you decide to break into the record label's archive. Because we can't have the actual master, we take the closest verifiable thing we can get our hands on and declare *that* our source. This is where things get spicy.

In the archiving world, your source usually comes from one of two main mediums: physical media rips (CD, Blu-ray, Vinyl, SACD) or, thanks to the internet, digital files sourced from streaming platforms (Apple Music, Tidal, Qobuz, Deezer) and digital storefronts (Bandcamp, HDtracks) - collectively referred to as WEB. All of them are also categorized as Analog and Digital Mediums. Let me quickly break down in short.

**Analog Physical Mediums:** Vinyl and Cassette tapes are the oldest form of music distribution; they are fundamentally analog. Vinyl stores the soundwave of your favorite album as a physical shape; literally cutting grooves in the vinyl disc. A needle traces those grooves and a cartridge translates the vibrations into electrical signals (analog), which pass through a phono preamp for correction and amplification, then into an amplifier, and finally to your speakers. To capture that signal digitally instead, an ADC intercepts it after the preamp to sample it into snapshots. The lossless/lossy framework doesn't cleanly apply here although lossless-ness of a vinyl disc can be judged by the condition of the disc (i.e. how many times it was played, what's the state of the disc after the plays, quality of the equipment used on it). The characteristics of a vinyl (like warmth, surface noise, dynamic range, impact on loudness war) and the debates around it are very interesting. More on that some other day. Moving on to Cassettes, a tape recorder alters the magnetization of magnetic tape in a cassette tape to record the soundwave. Unless it is the only source of a certain record, nobody really cares about cassettes anymore. They aren't 'lossy' in the digital sense, but they suffer from severe analog degradation, tape hiss, and physical generation loss every time you play them. A nightmare for preservation.

**Digital Physical Mediums:** Stepping out of analog and into digital, sound stops being a geometric shape and becomes numbers. Specifically, a very long list of numbers called PCM. Before we get into how that data actually works, let's look at the hardware.
YET TO WRITE





**WEB:** Digital files sourced from streaming platforms (Apple Music, Tidal, Qobuz, Deezer) and digital storefronts (Bandcamp, HDtracks) are collectively referred to as WEB. The convenience these platforms have brought is undeniable; we are getting files directly from the distributors themselves. No hassle of disc conditions or pressing quality. But they are not saints. Take *Wish You Were Here* by Pink Floyd. The original 1975 release was remastered in 1994. Then in 2011, James Guthrie remastered it again AND delivered a brand new stereo remix alongside a 5.1 surround mix. Then it got remastered once more in 2016. Four distinct versions of the same album across five decades. Log onto any major streaming platform today and you will find only one or two of them sitting there with no indication of which one it actually is. We have no idea if we're listening to the original mix or a remix or a remaster! Some will argue it is not sensible to host all four versions simultaneously. I would argue the opposite; hosting these pieces of history is any day more important than storing millions of AI slops on the same servers. That leads us to the authenticity, the *Hi-Res FLAC or ALAC* files on the platforms, are they truly what they claim to be? It might be rare for western distributors, but it's very common to find a 16 kHz hard cut-off file labelled *16-bit, 44.1 kHz* or even worse, *24-bit, 48/96/192 kHz* in Indian releases.

---

So what do these bits, kHz actually mean? Let's establish the units.
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
MORE TO WRITE. NYQUIST-SHANNON, CONTAINER RESOLUTION LOGIC

The Nyquist theorem states that to accurately reproduce a frequency, your sample rate needs to be at least twice that frequency. Since human hearing tops out at 20kHz, you need at minimum 40kHz. 44.1kHz gives you a little headroom. This is also why 44.1kHz is the universal baseline — it's the minimum sample rate that captures everything a human can hear, and nothing more than necessary.

Nyquist-Shannon sampling theorem says that to accurately reconstruct a continuous sound wave from those audio snapshots, your sample rate must be at least twice the highest frequency you want to capture. Going below that threshold will introduce aliasing - the wave folds back on itself and produces completely false frequencies that weren't in the original signal. If we want to capture as much as human ears can hear - that is 20 kHz, we have to double the sample rate to accurately capture the sound, at 40 kHz. That is why CD quality (44.1 kHz) is a standard; we get 4.1 extra kHz of sample rate that gives us a little breathing room - although the existence of those extra kilohertz in a CD is just a historical coincidence.

Earlier when we talked about Analog sound and Vinyl, I mentioned Analog-to-Digital Converter (ADC). When you "rip" a vinyl, you can set the ADC to capture at 24-bit/192kHz (you may have also seen some rips at 32-bit/384kHz or even at DSD64 to all the way up to DSD256). And it will absolutely fill that container. But what is it actually capturing? Most of the musical elements (vocals, instruments) naturally roll-off around 16-18 kHz. Everything above that is stylus noise, surface resonance, and ultrasonic cartridge artifacts. Technically real data from the vinyl, but not music.
Which raises another question, if your entire music is done by 18kHz, then what's the point of 48kHz, 96kHz or 192kHz? The point is headroom. Any mathematical artifacts that get generated by effects processing during the mixing (EQ curves, reverb tails, pitch correction, etc.) get pushed so far above the audible range that they're completely inaudible by the time the mix is rendered down to 44.1kHz. So aren't those extra sample rates unnecessary for me and shouldn't they be just stripped away after the production is complete? The answer is the moment you apply any kind of filter to remove content above any certain frequency - even the most mathematically perfect low-pass filter introduces phase artifacts at the edges of the cut - you've touched the signal and the cleanest thing you can do to a signal is to leave it untouched.

**Bit Depth & Dynamic Range**

When a computer takes a snapshot of a sound wave, it needs to store the height of the wave at that exact moment - the amplitude. But computers can't store infinite precision. They have to round the amplitude to the nearest available value. The tiny difference between the real value and the stored value becomes an error that accumulates across the whole recording. The rounding errors are called quantization noise. At low bit depths this is audible as distortion. At 16-bit it's below perception. At 24-bit it's essentially theoretical.

<details> <summary> Cool to know</summary>
A 1-bit system has only 2 possible values. On or off. The wave is either at maximum or at zero. Those 80s-90s crunchy video game sounds are an example of a 8-bit system that has 256 possible values. The wave exists but it's a rough approximation. The CD quality or a 16-bit system has 65,536 possible values. The rounding errors in this system are imperceptible to human ears under regular listening conditions. The rounding errors for a 24-bit system (16,777,216 possible values) are so small; they're buried beneath the noise floor of any real world listening environment.</details>

Every system has a floor and a ceiling. The ceiling is the maximum amplitude the system can store without distorting. Pushing past it introduces clipping - where the top of the sound wave gets chopped off. The floor is more interesting. It's not silence. It's the point where the audio signal becomes indistinguishable from the noise the system itself generates just by existing: hissing. When the music gets quiet enough to fall below that noise floor and disappears into it you hear hiss.
Dynamic range is the gap between those two points. How much distance exists between the noise floor and the clipping ceiling. Measured in decibels. Now here's where bit depth connects directly. Every bit you add to the system roughly doubles the number of amplitude values available, which pushes the noise floor down by about 6dB. More values means finer gradations means quieter quiets before the signal dissolves into noise. 16-bit gives you 96dB of dynamic range. 24-bit gives you 144dB. 16-bit covers most real world listening comfortably. 96dB covers everything from the quietest audible sound to a live concert. The extra headroom found in 24-bit matters most during recording and mixing; engineers need room to work without accidentally clipping any data.
The  rip of the very first and highly sophisticated Japanese CD pressing (The Black Triangle) for the album *The Dark Side Of The Moon*, which is 16-bit has more dynamic range than the 24-bit Vinyl rip of the "2011 Discovery Remaster". To answer why, let's shortly address the sneaky elephant in the room before finishing: Loudness War. 

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





### Codecs

### Spectrograms





**Transparency:** yes, LLMs were used. Not in a *"Write me an essay about lossy and lossless music files"* way, but to verify that my i's were dotted and t's were crossed. I do not have a degree in Sound Engineering; my main source of information was the internet. For debates, corrections or collectively hating on MQA, come to our telegram discussion group.
