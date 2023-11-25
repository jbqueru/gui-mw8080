# gui-mw8080
A fake GUI system running on Midway 8080 hardware 1975-1980
(used in a few dozen games including Gun Fight and Space Invaders.)

# Author
The primary author, primary maintainer, and primary copyright owner
of this code is Jean-Baptiste "JBQ" "Djaybee" Queru, member of the
MegaBuSTers demo crew.

# License
This software is Open Source,
licensed under the Apache License, Version 2.0

# Discussion

## Rationale

### What for
This project is centrally self-indulgent, where I (JBQ) want to
write code for some of the oldest hardware that I find interesting,
for no immediate purpose other than enjoying the challenge.

Additionally, this project explores questions of hardware
obsolescence for lack of software, aiming to partially replicate
experiences that arose in the mid-80s on hardware 10 years older,
which was a time period when hardware was evolving very quickly.
That discussion remains relevant to this day, where software
support cycles seem to terminate well before the matching hardware
has stopped working, which in turn creates situations where
reliability and repairability of consumer hardware keeps worsening
since there's no need any more to make hardware last in the face
of unsupported software. As evidence of that trend, even the EU's
legislative efforts for e-waste and cyberresilience seem to consider
that 5 years is an acceptable time horizon to replace hardware.

There is also an accessibility aspect, where the capabilities of
the original hardware are so limited that adopting accessibility
practices on that hardware creates interesting challenges.

### Why
The specific choice of this project is meant to eliminate exposure
to liability from GDPR and CRA, which totals 35 million Euros. The
chilling effect of such high fines keep me (JBQ) from contributing
to projects where such exposure might be higher.

### What
This project is meant to explore the potential capabilities of a
GUI system on limited hardware. The pixel count is 90% of that of
an Atari ST in low resolution mode, but it is limited to 1-bit
monochrome. Comparing again to an Atari ST, the CPU runs at a
quarter of the clock speed, takes slightly more clock cycles per
instruction, uses an 8-bit programming model instead of 32-bit,
and has a much simpler instruction set, with a single accumulator,
limited arithmetic, and primitive addressing modes.

A specific goal is to polish the display output, avoiding some of
the rough edges on the original Atari ST with its 8-bit-derived
fixed-width fonts and the graphics collisions in low resolution.

### Who
I (JBQ) am the primary author of this software, with support from
my artist wife who also has an interest in retrocomputing and
sustainability.

While contributions are also potentially accepted, I (JBQ) prefer
that potential contributors contact me ahead of time to discuss areas
of work. Specific areas of contributions include comments (where
someone reading the code without having written it might write
better comments) and testing (I honestly don't even know where to
start, many modern testing techniques seem hard to apply to such
low-level assembly).

### How
This software is hand-written in 8080 assembly, executed on an
emulator. Whether the code actually runs on real hardware isn't
immediately relevant.

### When
As I (JBQ) start to work on this project, in 2023, I am between
jobs and work on this code on my copious spare time. How much time
I will have in the future is unclear, such that any timeline for
this project should be taken with a grain of salt. It is explicitly
possible that this project might never finish or even reach basic
functionality.

## Licensing considerations

The original author (JBQ) initially toyed with the idea of using a
copyleft license, because he felt that there's so little software
available for that hardware that he'd love to see what people do
if they publish derivatives of his work. He had even released an
initial exploration under GPLv3.

He ended up coming back to Apache 2.0. He didn't want to use GPLv2
because of its incompatibility with Apache 2.0. He was worried about
the patent clause in (A)GPLv3, which he finds too broad. Additionally,
both GPLv2 and GPLv3 impose constraints on the development tools that
would get in the way of the expected development style of this software.

That being said, if someome makes changes to this work, the original
author would appreciate that the author of those changes distribute
the source code. If you do so, please update this README accordingly.

## Development environment
This software is developed against [8bitworkshop](https://8bitworkshop.com/).
Since 8bitworkshop uses [zmac](http://48k.ca/zmac.html) underneath,
it can probably be compiled directly with zmac as well.

Note: 8bitworkshop technically emulates a Z80, not an 8080.
While I try only to use 8080-compatible opcodes and mnemonics, that
alone doesn't guarantee that the code would work on a true 8080
environment (hardware or emulated.)

## Privacy (GDPR)
This software doesn't handle any personal data, by virtue of
having no identifiers and no information that would allow to
identify anyone. The original author doesn't recommend that
anyone modify this software to handle personal data, but, if
you do, you will be considered the controller for GDPR purposes.

## Cybersecurity (CRA)
This software doesn't have any direct or indirect network
connections. Also, it is non-commercial Open Source. Both of those
criteria are expected to put it outside the scope of the CRA.
Additionally, the original author contributes to this software
on an individual basis, not in the context of any contract or
employment.

That being said, the development process stops at "it works on
one emulator" and is far from modern best practices. The
original author doesn't recommend that you modify this software
for use in an environment where cybersecurity is important, but,
if you do, this will be considered a significant modification for
CRA purposes.
