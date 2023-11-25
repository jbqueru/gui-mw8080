# gui-mw8080
A fake GUI system running on Midway 8080 hardware 1975-1980
(Gun Fight to Space Invaders.)

# Author
The primary author, primary maintainer, and primary copyright owner
of this code is Jean-Baptiste "JBQ" "Djaybee" Queru, member of the
MegaBuSTers demo crew.

# License
This repository is licensed under Apache v2.0.

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

# Development environment
This software is developed against [8bitworkshop](https://8bitworkshop.com/).
Since 8bitworkshop uses [zmac](http://48k.ca/zmac.html) underneath,
it can probably be compiled directly with zmac as well.

Note: 8bitworkshop technically emulates a Z80, not an 8080.
While I try only to use 8080-compatible opcodes and mnemonics, that
alone doesn't guarantee that the code would work on a true 8080
environment (hardware or emulated.)

# Privacy (GDPR)
This software doesn't handle any personal data, by virtue of
having no identifiers and no information that would allow to
identify anyone. The original author doesn't recommend that
anyone modify this software to handle personal data, but, if
you do, you will be considered the controller for GDPR purposes.

# Cybersecurity (CRA)
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
if you do, that'll be considered a significant modification for
CRA purposes.
