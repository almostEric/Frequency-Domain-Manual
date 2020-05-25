
# Frequency Domain VCV plugins

Frequency domain based VCV Plugins

## Freudian Slip
![Frudian Slop](./doc/freudian_slip.png)

- Sample based Spectral Resyntheszer
- Right click to load sample
- Analyzes the sample's spectal content and then drives up to 32 oscillators based on that analysis
- Right click to adjust Windowing Function which alters harmonic content  
- Right click on grids to choose from default shapes or transform patterns
- Speed cobtrols the speed or duration of the playback without changing pitch
- Negative play speeds play sample in reversse
- By drawing a curve, each voice can have its own play speed - even ones where some voices go forwards, others in reverse
- Voice Count specifies how many oscillators are used (1-32)
- Waveform specifies what waveform the oscillators output
- Frequency Warp pushes oscilator's frequency away from CENTER frequency 
- If the V1 switch is on, the center frequency tracks the main oscillator and CENTER control adds an offset  
This is great for creating inharmonic sounds
- Frequency Modulation inputs are polyphonic. You can have up to 32 FM inputs (using both FM inputs). 
- Randomize controls amount of randoming stepping between frames
- FM Matrix controls which FM input (x axis) modulates which oscillator (y axis).
- FM Amount allows per oscillator FM control
- RM/AM inputs are polyphonic. You can have up to 32 inputs (using both RM/AM inputs).  
- RM/AM Matrix controls which AM/RM input (x axis) modulates which oscillator (y axis).
- AM/RM Mix controls the amount of amplitude modulation 
- Panning allows each oscillator to be placed in the stereo field
- X AND Y inputs on all grids allow CV Modulation of grid in either dimension
- Panning and Play Speed grids have rotate CV input that rotates x values around the y axis


## Harmonic Convergence
![Harmonic Convergence](./doc/harmonic_convergence.png)

- Live Spectral Resyntheszer
- Takes one or two inputs, analyzes their spectal content and then drives up to 36 oscillators based on that analysis
- Right click to adjust Windowing Function and each inputs' Frame Size  
Smaller frame sizes handle transients (like drums and speech beter), but the pitch becomes less accurate   
Large frame sizes more accurately detect pitch, but can make some input sounds seem like they have reverb
- Right click on grids to choose from default shapes or transform patterns
- The Morph panel controls the how much each input contributes to each individual osccilator.
- Voice Count specifies how many oscillators are used (1-36)
- Waveform specifies what waveform the oscillators output
- Frequency Shift shifts all oscillators +/- 3 octaveas
- Frequency Warp pushes oscilator's frequency away from CENTER frequency 
- If the V1 switch is on, the center frequency tracks the main oscillator and CENTER control adds an offset  
This is great for creating inharmonic sounds
- Spectral Mode changes how the most prominent frequency bands drive the voice oscillators
- Voice Shift allows the magnitude of one frequency to control another
- Frequency Modulation inputs are polyphonic. You can have up to 32 FM inputs (using both FM inputs). 
- FM Matrix controls which FM input (x axis) modulates which oscillator (y axis).
- FM Amount allows per oscillator FM control
- RM/AM inputs are polyphonic. You can have up to 32 inputs (using both RM/AM inputs).  
- RM/AM Matrix controls which AM/RM input (x axis) modulates which oscillator (y axis).
- If Internal is turned on the RM Matrix allows oscillators to Ring Modulate one another. 
- AM/RM Mix controls the amount of amplitude modulation 
- In Internal mode, AM/RM Mix controls the blend between the original oscillator voice and the results of ring modulation 
- Panning allows each oscillator to be placed in the stereo field
- X AND Y inputs on all grids allow CV Modulation of grid in either dimension

## Delayed Reaction
![Delayed Reaction](./doc/delayed_reaction.png)

- In loving memory of Native Instrument's Spektral Delay.
- Each frequency band can have its own initial volume level, delay time and feedback amount
- Right click to adjust Windowing Function and Frame Size
- Right click on grids to choose from default shapes or transform patterns
- Send and Return allow the Feedback to be further processed
- 2 or more Delayed Reactions can be used as expanders. When the LINK is enabled, drawing a curve on the master DR copies it to the others.
- PINxs have five modes
  * Off - PinX control has no effect
  * Light Green - values (without CV) less than pinX axis are set to pinXs value, otherwise use value (+ cv)
  * Green - values (without CV) less than pinX axis are unchanged, otherwise use value (+ cv)
  * Pink - values (without CV) greater than pinX axis are set to pinXs value, otherwise use value (+ cv)
  * Red - values (without CV) greater than pinX axis are unchanged, otherwise use value (+ cv)
- Rotation allows rotating x values around the oinX axis

## Morphology
![Morphology](./doc/morphology.png)

- Essentially a spectral based vocoder.
- Frequency bands can be placed individually in the stereo field
- Band spread allows frequency bands to modulate their neighbors.
- Inverter buttons make loudest frequency bands the quietest and vice-versa
- Each input has a CV controllable Invert threshold which determines how loud a band must be for it to be inverted.  
At low thresholds the input can become very noisey  
- Right click to adjust Windowing Function and Frame Size
- Right click on grids to choose from default shapes or transform patterns
- Rotation allows rotating x values around the oinX axis
