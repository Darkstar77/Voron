# TAP
---
I've been working on a problem between the LDO MGN12H carriage, and the TAP centre causing the belts to slip. The TAP centre is designed with the assumption the ends caps are flush with the main body of the carriage. Reported and documented here:

https://github.com/VoronDesign/Voron-Tap/issues/51

I have designed a spacer, which worked until it deformed. It is very hard to print, requiring a very thin first layer, and needs to be overextruded.

In addition, I have been revising the actual TAP centre to compensate for the difference in the LDO carriage and what it has been designed for. The gap is 0.6mm, which I am attempting to compensate for by increasing raising the teeth that engage the belt by 0.4mm and increasing the should height be 0.2mm. Still testing the idea, so this is alpha, beta at best.

![Original TAP Center Beside Modified](./OriginalCentreNewCentre.png?raw=true)
