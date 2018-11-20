# video-audio-generator

Generates sound using Python and PureData. The openCV library, for Python, is used to capture video from a Playstation Eye camera, finds the average color for a given frame, then assigns a note from the C major scale to the average, and sends the assigned note to PureData. 

The PureData file consists of a simple oscillator, that outputs third octave notes sent from the Python script.

## Next Steps

As this is intended to run on a Raspberry Pi attached to the bottom of a skateboard, there will be a function for assigning octaves to notes based on the board's rate of speed. Alternatively, the board's rate of speed could be used to assign RPM. Also, rather than assigning a note to a frames color average, a given frame will be split into seven rows, and the color average of each row will generate a note, sending 7 notes at a time.

