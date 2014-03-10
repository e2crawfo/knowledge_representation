### Biologically inspired methods in speech recognition and synthesis:

### Closing the loop

Trevor Bekolay <br>
Centre for Theoretical Neuroscience



img: Speech recognition silo, speech synthesis silo

then they break... maybe by a falling brain?

Note: Current approach to auditory processing in CS.



img: long-term goal model of recognition / synthesis hierarchies
(this would be different from in the proposal)

Note: Ideal long-term goal of this line of research



img: short-term goal model of voicing a small vocabulary

Note: My project!



img: template learning details

Note: Let's talk about the "recognition" part.
The idea is to build up a "template" of what each
word in the vocabulary sounds like,
so that we can later try to mimic it.



img: Speech recognition basics

Note: Here's how computers do it.



img: human auditory periphery

img: zilany model

Note: We're going to use a biologically plausible frontend,
which may give some benefits for accuracy, but is also
for keeping information in the same format.



img: classifier

Note: This has been done before, but now we're incorporating
temporal information. Look up the RNN thing...



img: path integrator

Note: Oliver's stuff



img: template memory

Note: Some kind of averaging of nonlinearities?



img: motor learning details

Note: Okay, so now we've got a list of words and a template
of what each word sounds like. Now we want to mimic that sound.



img: Birkholz synthesizer

Note: We'll do this, again, in a biologically plausible way;
this thing models the human vocal tract.



img: show Birkholz parameters

Note: However, it's a 23-degree of freedom control problem.
That's not good. People have learned to control it relatively well though.



audio: Birkholz synthesis examples

Note: Here are some examples. Done by looking at detailed MRI images.



img: motor learning through reinforcement

Note: We should probably start from there, but then we should
get better through reinforcement.
We can tell how good we're doing by comparing our utterance to
the template utterance.
