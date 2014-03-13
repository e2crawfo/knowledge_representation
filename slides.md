### Biologically inspired methods in speech recognition and synthesis:

### Closing the loop

Trevor Bekolay <br>
Centre for Theoretical Neuroscience <br>
Follow along: <http://bekolay.org/comp2>

---Right---

Speech recognition and synthesis is everywhere

<iframe src="http://talktyper.com/" width="800"></iframe>

---Right---

<object type="image/svg+xml" data="img/silos.svg" width="500"></object>

<object type="image/svg+xml" data="img/recognition.svg" width="890" class="fragment"></object>

---Right---

<object type="image/svg+xml" data="img/longterm.svg" width="700"></object>

---Down---

<object type="image/svg+xml" data="img/kroger.svg" width="550"></object>

----

<small>Towards a neurocomputational model of speech production and
perception.<br>Kroger et al. *Speech Communication*, **51**(9):793–809,
2009.</small>

---Right---

<object type="image/svg+xml" data="img/birdsong.svg" width="800"></object>

----

<small>Neural network models of birdsong production, learning, and
coding.<br>Fiete & Seung. In *The New Encyclopedia of
Neuroscience*(New York: Elsevier), 2008.</small>

---Right---

<object type="image/svg+xml" data="img/shortterm.svg" width="800"></object>

---Right---

<object type="image/svg+xml" data="img/template.svg" width="600"></object>

---Right---

<object type="image/svg+xml" data="img/periphery-anatomy.svg" width="890"></object>

---Right---

<object type="image/svg+xml" data="img/zilany.svg" width="890"></object>

----

<small>A phenomenological model of the synapse between the inner hair
cell and auditory nerve: long-term adaptation with power-law
dynamics.<br>Zilany, et al. *The Journal of the Acoustical Society
of America*, **126**:2390–2412, 2009.</small>

---Right---

<object type="image/svg+xml" data="img/template.svg" width="600"></object>

---Right---

$$\Delta \omega\_{ij} \propto a\_i [S
  \underbrace{e\_j \cdot E}\_{\color{blue}{\text{ Supervised}}}
  + (1 - S) \,
  \underbrace{a\_j (a\_j - \theta)}\_{\color{blue}{\text{ Unsupervised}}}]$$

<br><object type="image/svg+xml" data="img/ctc.svg" width="800" class="fragment"></object>

----

<small>Connectionist temporal classification: labelling unsegmented
sequence data with recurrent neural networks.<br>Graves et al. In
*Proceedings of the 23rd international conference on Machine
learning*, pages 369–376. ACM, 2006.<br><br>
Simultaneous unsupervised and supervised learning of cognitive
functions in biologically plausible spiking neural networks.<br>Bekolay
et al. In *Proceedings of the 35th Annual Conference of the Cognitive
Science Society*, pages 169–174, 2013.</small>

---Right---

<object type="image/svg+xml" data="img/template.svg" width="600"></object>

---Right---

<object type="image/svg+xml" data="img/path-integrator.svg" width="600"></object>

----

<small>A controlled attractor network model of path integration in the
rat.<br>Conklin & Eliasmith. *Journal of Computational Neuroscience*,
**18**:183–203, 2005.</small>

---Right---

<object type="image/svg+xml" data="img/template.svg" width="600"></object>

---Right---

<object type="image/svg+xml" data="img/trajectory-average.svg" width="890"></object>

----

<small>Stimulus onset quenches neural variability: a widespread
cortical phenomenon.<br>Churchland et al. *Nature Neuroscience* **13**,
369-378, 2010</small>

---Right---

<object type="image/svg+xml" data="img/motor.svg" width="400"></object>

---Right---

<object type="image/svg+xml" data="img/birkholz.svg" width="750"></object>

----

<small>Modeling consonant-vowel coarticulation for articulatory speech
synthesis.<br>Birkholz. *PloS one*, **8**(4):e60603, 2013.</small>

---Right---

<div style="display:inline-block; width:320px;">
  <video width="320" height="240" controls preload="auto">
    <source src="media/guten-tag.ogg" type="video/ogg">
  </video>
</div>

<div style="display:inline-block; width:500px; text-align:left;">
  <audio controls preload="auto">
    <source src="media/s1-neutral.wav" type="audio/wav">
  </audio>
  Normal

  <audio controls preload="auto">
    <source src="media/s1-anger.wav" type="audio/wav">
  </audio>
  <span class="secret">Angry</span>

  <audio controls preload="auto">
    <source src="media/s1-boredom.wav" type="audio/wav">
  </audio>
  <span class="secret">Bored</span>

  <audio controls preload="auto">
    <source src="media/s1-disgust.wav" type="audio/wav">
  </audio>
  <span class="secret">Disgusted</span>

  <audio controls preload="auto">
    <source src="media/s1-fear.wav" type="audio/wav">
  </audio>
  <span class="secret">Scared</span>

  <audio controls preload="auto">
    <source src="media/s1-happiness.wav" type="audio/wav">
  </audio>
  <span class="secret">Happy</span>

  <audio controls preload="auto">
    <source src="media/s1-sadness.wav" type="audio/wav">
  </audio>
  <span class="secret">Sad</span>
</div>

----

<small>
<http://www.vocaltractlab.de/index.php?page=vocaltractlab-examples> <br>
<http://www.vocaltractlab.de/index.php?page=birkholz-supplements>
</small>

---Right---

<video width="500" controls preload="auto">
  <source src="media/dona-nobis.ogg" type="video/ogg">
</video>

<video width="500" controls preload="auto">
  <source src="media/salvete.mp4" type="video/mp4">
</video>

----

<small>
<http://www.vocaltractlab.de/index.php?page=vocaltractlab-examples> <br>
<http://www.vocaltractlab.de/index.php?page=birkholz-supplements>
</small>

---Right---

<table id="birkholz-params" class="reveal">
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

---Right---

![Operational space control](img/osc.gif)

---Right---

<object type="image/svg+xml" data="img/learn-osc.svg" width="890"></object>

----

<small> Learning to control in operational space.<br> Peters & Schaal.
*The International Journal of Robotics Research* **27**(2), 197-212,
2008 </small>

---Right---

## Thank you

This presentation: <http://bekolay.org/comp2>

My progress: <http://github.com/tbekolay/audition>
