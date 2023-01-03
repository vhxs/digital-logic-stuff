### Decade counter with a 7-segment display
(I know this is upside down...)

https://user-images.githubusercontent.com/93892166/210297976-e50a5362-fbfe-4d7c-acd4-357fcbff162b.mov

Adds a 7-segment display to show digits instead of bits. The 4 bits of output are passed to a 74LS47 BCD-to-7-segment decoder. This IC has active low outputs, so each is fed through a NOT gate before being passed to the individual segments of the display.
