# Forensics Day 2


Hey guys, so following Day 1, you guys are now set up with Kali in VirtualBox. 

What is [Forensics](https://www.sentinelone.com/cybersecurity-101/cybersecurity/cybersecurity-forensics/)?

So moving to forensics, in my opinion, it is the most brain-scratching, random domain. The amount of random, unhinged variations you can do to a challenge and still keep it under the "forensics" domain is crazy.

Broadly, there are 3-4 major sub-subdomains in this subdomain.
1. Image forensics
2. Audio forensics
3. Network forensics
4. Memory forensics

We will talk majorly about the first two here and some little random facts here and there. 

The tools mentioned below should already be installed in your Kali systems. If not just google how to do it :)

So here, we play with files, right? Every file has some metadata associated with it - what, where, who created it, File signatures etc etc.

Every file is somewhat similar when it comes to the basic structure.
Analyzing the metadata, one sees the file signatures which can be mapped to the kind of file it is. Some files also contain starting and ending bytes which help us to sense if the file is corrupt or not.

First of all what is [steganography](https://www.geeksforgeeks.org/computer-networks/what-is-steganography/)?
Read [this](https://ryanagibson.com/posts/steganography-intro/) too.

#### Image forensics
Watch [this](https://youtu.be/TWEXCYQKyDc?si=azPyj3EDm88fhfZa) video for an introduction to Image steganography.

1st rule of forensics, any file that you have obtained, apply the `strings` and `exiftool` command to it and search it for something "interesting". 

Few ways to hide stuff in images:
1. Appending stuff at the end of for example a .png image
2. [LSB steganography](https://medium.com/@renantkn/lsb-steganography-hiding-a-message-in-the-pixels-of-an-image-4722a8567046) 
3. Layering the hiding of stuff - like audio in image etc

Coming to the tools,
1. binwalk - first is binwalk, it works pretty well for finding things embedded between the files. But one thing is that it doesn't work on .jpeg images and I can't seem to extract the hidden audio files using this.
2. steghide - steghide is the binwalk-alternative when working with .JPEGs
3. zsteg - it detects the LSB stego along with a few other things
4. [sherloq](https://github.com/GuidoBartoli/sherloq)
5. [Aperisolve](https://www.aperisolve.com/) - In the beginning, you won't even need the above tools. But moving further, it becomes rather moody.

#### Audio forensics
What is this thing? See [this](https://www.youtube.com/watch?v=rAGkm4pv44s).
Two things I come across frequently here is Morse code and audio spectrogram. 
Tools:
1. Audacity - "easy-to-use, multi-track audio editor and recorder" I use it to view the spectrogram of the audiofile. 
"A spectrogram is a picture of sound. A spectrogram shows the frequencies that make up the sound, from low to high, and how they change over time, from left to right." 
[Here's](https://medium.com/@AungKyawZall/audio-steganography-39f9fb6d9330) how you can hide text yourself in an audio file.
2. Ascii-to-Morse-audio converters
3. [DTMF tones](https://en.wikipedia.org/wiki/DTMF) - [this](https://github.com/ribt/dtmf-decoder) tool can be used along with a variety of online applications that are now available.
4. [wavsteg](https://github.com/ragibson/Steganography#WavSteg)
5. [Sonic Visualiser](https://www.sonicvisualiser.org/)

#### Other tools
1. [HexEditor](https://hexed.it/)
2. [This](https://29a.ch/photo-forensics/#forensic-magnifier)
3. [Read](https://github.com/cyberteach360/Steganography)
4. [Chess steganography](https://incoherency.co.uk/blog/stories/chess-steg.html) - If you like chess.


For the rest of the topics, you can go through the PClub InfoSec roadmap [here](https://pclub.in/roadmap/2024/06/06/infosec-roadmap/).

Most of the times, the challenge would be a mix of all these things. So one should be able to identify what is what, how can they be mixed into one another. 

**I know this is A LOT for a day, so try to get a feel for how forensics is, its applications. Learnathon is supposed to just be the introduction to the domains, so don't worry about it if you don't complete.**



