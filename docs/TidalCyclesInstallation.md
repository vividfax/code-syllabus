# Tidal Cycles Installation

- [MacOS automated installation](https://tidalcycles.org/MacOS_automated_installation)
- [Start tidalcycles and superdirt for the first time](https://tidalcycles.org/Start_tidalcycles_and_superdirt_for_the_first_time)

If you get this error: `ERROR: Input sample rate is 44100, but output is 48000. Mismatched sample rates are not supported. To disable input, set the number of input channels to 0.` Then paste the following code into the SuperCollider window, click on the code, and hold down shift and press enter for each of the lines.

```
Server.local.options.sampleRate = 44100;
Server.internal.options.sampleRate = 44100;
```

Then run `SuperDirt.start` again.
