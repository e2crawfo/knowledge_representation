### Biologically inspired methods in speech recognition and synthesis:

### Closing the loop

Trevor Bekolay <br>
Centre for Theoretical Neuroscience



img: Speech recognition silo, speech synthesis silo

then they break... maybe by a falling brain?

Note: Current approach to auditory processing in CS.



<object type="image/svg+xml" data="img/longterm.svg" width="800"></object>

(make different from in the proposal)

Note: Ideal long-term goal of this line of research


<object type="image/svg+xml" data="img/kroger.svg" width="800"></object>

----

<small>Towards a neurocomputational model of speech production and
perception. Kroger et al. *Speech Communication*, **51**(9):793–809,
2009.</small>



<object type="image/svg+xml" data="img/shortterm.svg" width="890"></object>

Note: My project!



<object type="image/svg+xml" data="img/template.svg" width="600"></object>

Note: Let's talk about the "recognition" part.
The idea is to build up a "template" of what each
word in the vocabulary sounds like,
so that we can later try to mimic it.



<object type="image/svg+xml" data="img/recognition.svg" width="890"></object>

Note: Here's how computers do it.



<object type="image/svg+xml" data="img/periphery-anatomy.svg" width="890"></object>



<object type="image/svg+xml" data="img/zilany.svg" width="890"></object>

----

<small>A phenomenological model of the synapse between the inner hair
cell and auditory nerve: long-term adaptation with power-law
dynamics. Zilany, et al. *The Journal of the Acoustical Society
of America*, **126**:2390–2412, 2009.</small>

Note: We're going to use a biologically plausible frontend,
which may give some benefits for accuracy, but is also
for keeping information in the same format.



$$\Delta \omega\_{ij} \propto a\_i [S
  \underbrace{e\_j \cdot E}\_{\color{blue}{\text{ Supervised}}}
  + (1 - S) \,
  \underbrace{a\_j (a\_j - \theta)}\_{\color{blue}{\text{ Unsupervised}}}]$$

img: rnn

----

<small>Simultaneous unsupervised and supervised learning of cognitive
functions in biologically plausible spiking neural networks. Bekolay
et al. In *Proceedings of the 35th Annual Conference of the Cognitive
Science Society*, pages 169–174, 2013.</small>

Note: This has been done before, but now we're incorporating
temporal information. Look up the RNN thing...



<object type="image/svg+xml" data="img/path-integrator.svg" width="600"></object>

----

<small>A controlled attractor network model of path integration in the
rat. Conklin & Eliasmith. *Journal of Computational Neuroscience*,
**18**:183–203, 2005.</small>

Note: Oliver's stuff



<object type="image/svg+xml" data="img/trajectory-average.svg" width="890"></object>

----

<small>Stimulus onset quenches neural variability: a widespread
cortical phenomenon. Churchland et al. *Nature Neuroscience* **13**,
369-378, 2010</small>

Note: Some kind of averaging of nonlinearities?



<object type="image/svg+xml" data="img/motor.svg" width="400"></object>

Note: Okay, so now we've got a list of words and a template
of what each word sounds like. Now we want to mimic that sound.



<object type="image/svg+xml" data="img/birkholz.svg" width="800"></object>

Note: We'll do this, again, in a biologically plausible way;
this thing models the human vocal tract.



<table id="birkholz-params">
  <tr>
    <th>Name</th>
    <th>Description</th>
    <th>Min.</th>
    <th>Max</th>
    <th>Unit</th>
  </tr>
  <tr>
    <td>$HX$</td>
    <td>Horizontal hyoid position</td>
    <td>0.0</td>
    <td>1.0</td>
    <td></td>
  </tr>
  <tr>
    <td>$HY$</td>
    <td>Vertical hyoid position</td>
    <td>-6.0</td>
    <td>-3.4</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$JX$</td>
    <td>Horizontal jaw displacement</td>
    <td>-0.5</td>
    <td>0.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$JA$</td>
    <td>Jaw angle</td>
    <td>-7.0</td>
    <td>0.0</td>
    <td>deg</td>
  </tr>
  <tr>
    <td>$LP$</td>
    <td>Lip protrusion</td>
    <td>-1.0</td>
    <td>1.0</td>
    <td></td>
  </tr>
  <tr>
    <td>$LD$</td>
    <td>Vertical lip distance</td>
    <td>-2.0</td>
    <td>4.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$VS$</td>
    <td>Velum shape</td>
    <td>0.0</td>
    <td>1.0</td>
    <td></td>
  </tr>
  <tr>
    <td>$VO$</td>
    <td>Velic opening</td>
    <td>-0.1</td>
    <td>1.0</td>
    <td></td>
  </tr>
  <tr>
    <td>$TCX$</td>
    <td>Tongue body center X</td>
    <td>-3.0</td>
    <td>4.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TCY$</td>
    <td>Tongue body center Y</td>
    <td>-3.0</td>
    <td>1.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TTX$</td>
    <td>Tongue tip X</td>
    <td>1.5</td>
    <td>5.5</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TTY$</td>
    <td>Tongue tip Y</td>
    <td>-3.0</td>
    <td>2.5</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TBX$</td>
    <td>Tongue blade X</td>
    <td>-3.0</td>
    <td>4.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TBY$</td>
    <td>Tongue blade Y</td>
    <td>-3.0</td>
    <td>5.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TRX$</td>
    <td>Tongue root X</td>
    <td>-4.0</td>
    <td>2.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TRY$</td>
    <td>Tongue root Y</td>
    <td>-6.0</td>
    <td>0.0</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TS1$</td>
    <td>Tongue side elevation 1</td>
    <td>-1.4</td>
    <td>1.4</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TS2$</td>
    <td>Tongue side elevation 2</td>
    <td>-1.4</td>
    <td>1.4</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TS3$</td>
    <td>Tongue side elevation 3</td>
    <td>-1.4</td>
    <td>1.4</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$TS4$</td>
    <td>Tongue side elevation 4</td>
    <td>-1.4</td>
    <td>1.4</td>
    <td>cm</td>
  </tr>
  <tr>
    <td>$MA1$</td>
    <td>Minimum area tongue back region</td>
    <td>0.0</td>
    <td>0.3</td>
    <td>cm$^2$</td>
  </tr>
  <tr>
    <td>$MA2$</td>
    <td>Minimum area tongue tip region</td>
    <td>0.0</td>
    <td>0.3</td>
    <td>cm$^2$</td>
  </tr>
  <tr>
    <td>$MA3$</td>
    <td>Minimum area lip region</td>
    <td>0.0</td>
    <td>0.3</td>
    <td>cm$^2$</td>
  </tr>
</table>

Note: However, it's a 23-degree of freedom control problem.
That's not good. People have learned to control it relatively well though.



audio: Birkholz synthesis examples

Note: Here are some examples. Done by looking at detailed MRI images.



img: motor learning through reinforcement

Note: We should probably start from there, but then we should
get better through reinforcement.
We can tell how good we're doing by comparing our utterance to
the template utterance.
