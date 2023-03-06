# TAP
---
I've been working on a problem between the LDO MGN12H carriage, and the TAP centre causing the belts to slip. The TAP centre is designed with the assumption the ends caps are flush with the main body of the carriage. Reported and documented here:

https://github.com/VoronDesign/Voron-Tap/issues/51

I have designed a spacer, which worked until it deformed. It is very hard to print, requiring a very thin first layer, and needs to be overextruded.

In addition, I have been revising the actual TAP centre to compensate for the difference in the LDO carriage and what it has been designed for. The gap is 0.6mm, which I am attempting to compensate for by raising the teeth that engage the belt by 0.4mm and increasing the shoulder height by 0.2mm. Still testing the idea, so this is alpha, beta at best.

![Original TAP Center Beside Modified](./OriginalCentreNewCentre.png?raw=true)

---

## Installation & Assembly Notes/ Tips

Part of the issue I've seen with the TAP center part, is that during assembly you are performing a preliminary tensioning of the belts, when you bolt the center to the rail carriage. If the teeth of the 2GT belt are even partially engaged with the centre teeth, and you pull the belts through to tension them, you are going to damage the teeth on the center. I have experienced this failure, and the resulting belt slip that comes with it during tensioning or when printing.

If you keep this in mind, you can assemble this without damaging the center. Here is what I recommend: 
1. Install both belts on one side, thread them through, all the way through the securing tabs, and make sure they have engaged the teeth fully. At this stage you should have the belts on one side fully seured, so they will not move. 
2. Now, carefully thread the other belts into the centre on the opposite side, but while doing this, take extra caution to prevent the 2GT belt from engaging the teeth on the center, until the belts are tensioned as much as reasonable and evenly tensioned. 
3. Engage the teeth, and carefully hold the center so the belts cannot move. 
4. Bolt the centre to the carriage, taking extra care to not move the 2 unsecured belts. Evenly snug, then tighten the bolts to avoid excess stress on the part.
5. Thread the belt through the securing tabs to fully secure them.
6. Derack and tension the belts. Do this now, not later. If your belts are going to slip, it's most likely going to happen now.

From my perspective, about 50% of the issue is during assembly, and damaging those teeth. The other half is all of those MGN12H carriages with endcaps that are not flush with the carriage itself.

---

## Update

In the STL folder there are two revisions on the TAP centre, TAP_Centre_R6_LDORail.stl & TAP_Centre_R6.2_LDORail.stl. The first is pictured above, which does as described, and takes away most of the space between the carriage end caps, and the centre part. This worked for me. I've been running it now for about 30 hours of printing, and it's working fine. I did note some stress on the "wings" where the belts mount however.

This led me to design the second revision, which I have printed, but not installed yet. It changes the proportions a little, as well as changes the profile on the teeth to increase their strength a little. I have confirmed 2GT belt fits it just fine, and based on my testing with the original, it should work the same, without stressing the wings of the centre as much. Here is the original vs my latest revision:

![Original TAP Center Beside R2 Modified](./R6.2-vs-original.png?raw=true)
