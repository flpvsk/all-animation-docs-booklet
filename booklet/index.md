# akkusativ
## All Animation


#### TOC

* Overview
* Block Diagram
* Details by section
    * Routing
    * FADE
    * FLIP
    * TRACE
* Patch Ideas
    * Gated Anything
    * Dirt Body – Clean Tail
    * Feedback System
* Technical Details
* Repair
* End of Life
* Commitment to Open Source


#### Overview

All Animation is a crossfader, a signal router and an
envelope follower. Use it to build your own dynamic effects
and feedback machines: mixers, gates, auto-swell and tremolo
effects. Control it using CV or Expression, or use *it* to
control other CV-enabled devices.

The `FADE` section lets you combine signals coming from two
effect chains and control the mix using knobs, footswitches
and voltages.

The `route` toggle lets you choose between running effects
in parallel or in series.

The `TRACE` section is an envelope follower that outputs the
loudness of a signal as a voltage. You can use that voltage
to control other parts of All Animation or external gear.
Trace the pedal input, one of the returns or an external
signal.

<!-- Fig. 1 Block Diagram -->

#### Routing

There are several options for routing using All Animation:

* `IN -> A SEND` | `IN       -> B SEND`
* `IN -> A SEND` | `A RETURN -> B SEND`
* `IN -> B SEND` | `B RETURN -> A SEND`

<!-- Fig. 2 route switch positions -->

On the default setting, with the `route` switch in the
center position, the `IN` signal is split and sent into `A
SEND` and `B SEND`. This setting is for running effects in
parallel.

The other two settings send the output of one chain into the
other chain. Use them for running effects in series.

All Animation also has a second always active output (marked
`A~B`). It has the exact same signal as `OUT`, except it is
not affected by the `BYPASS` switch. Use it for making
feedback patches.

Some effects will invert the phase of the input signal, and
that will affect the mix when running them in parallel. Use
the phase switch to invert the phase of `B RETURN`.

#### FADE

FADE lets you gradually crossfade between `A RETURN` and
`B RETURN` signals. Use the range knob by itself or in
combination with an expression pedal or a CV source to
control the position of the crossfade.

> **DIP-switch: expr.**
>
> By default the FADE input jack is set up to take CV only,
> not expression. That way you can use normal TS (mono) patch
> cables for that input. If you'd like to use it with an
> expression pedal, flick the expression dip-switch on the
> inside of the pedal to the ON position. In that case you
> can use the input with both CV and expression, but you would
> have to use TRS (stereo) patch cables for the FADE input.

The range knob acts as an attenuverter: the range of the
fade curve is going to be zero when the knob is at noon.
In that position, both `A RETURN` and `B RETURN` signals will
be at 100% independently of the CV or Expression going into
the FADE input jack. In the fully counter-clockwise position,
CV values 0V to 5V would fade from 100% `A RETURN` to 100%
`B RETURN`. When the range is full clockwise, the direction
of the fade is reversed.

<!-- Fig. 3 Fade curve -->

You don't have to use the FADE input jack to do the
crossfading. With nothing inserted, the pedal would go
between full `A RETURN` with the range knob
counter-clockwise to full `B RETURN` with the knob turned
clockwise.

> **DIP-switch: smooth**
>
> The FADE input jack is sensitive, sometimes too sensitive.
> If you hear unpleasant scratchy noises when using an
> expression pedal, flick the smooth DIP-switch on the
> inside of the pedal to the ON position.



#### FLIP

`FLIP` lets you smoothly reverse the position on the FADE
curve. 20-80 fade becomes 80-20, 45-55 becomes 55-45 and so on.
The attack knob controls how fast the `FLIP` happens. The
release knob – the time it takes to settle back into the
original position on the FADE curve once the `FLIP` is
disengaged.

<!-- Fig. 3 Flip curve -->

`FLIP` can be triggered via the footswitch or via a 5V gate
input.

> Tip: plug in a gate sequencer into `FLIP` to move
> between effect chains in time with the main beat of the
> song.

> Tip: plug in the TRACE output into `FLIP` to create dynamic
> effects: compressors, expanders, auto-swells. Plug in an
> external signal into TRACE input for a sidechain
> effect.

#### CYCLE

It is possible to `CYCLE` the `FLIP`. That way the pedal would
move back and forth on the fade curve with the speed
controlled by the attack and release knobs, the depth
controlled by the original position on the FADE curve.

> Tip: unplug one of the returns and press `CYCLE` to create a
> tremolo effect.

#### TRACE

`TRACE` is an envelope follower. Use it to turn the
dynamics of your `IN`, `A RETURN`, `B RETURN` or external
signal into control voltage. Patch that control voltage
back into All Animation to create gate, compressor and
swell-type effects or send it into external gear.

<!-- Fig. 4 TRACE form switch positions -->

The `sens` knob controls the sensitivity of the envelope
follower. The `form` toggle controls the shape of the TRACE
output. The options are gate, continuous or trigger.

> Tip: Patching an external signal into `TRACE IN` gives you
> a sidechain: a way to control the FADE or `FLIP` section
> using the dynamics of that external signal.

#### Patch Ideas: Gated Anything

Use this patch when you want an intense effect to be present
only when you play and fade out when you stop.

Change the TRACE output switch to the gate option and run
TRACE out into `FLIP` in for more control over onset and
completion of the transition.

#### Patch Ideas: Dirt Body – Clean Tail

A good occasion to run effects in parallel is when you want a
sound with an aggressive / compressed attack and gentle
tails. Here the input signal runs through both dirt section
and time-based effects. You get the best of both as a
result.

#### Patch Ideas: Feedback System

Run any effect chain into itself with `A~B` output. Use the
gain controls and the `FADE` section to control the amount
of feedback. Use the `TRACE` section to control that
feedback loop in response to the input or other signal.

#### Technical Details

* Dimensions: 145mm x 130mm x 70mm (5.7in x 5.1in x 2.8in)
* Power: 9VDC 150mA
* Impedance of audio inputs (IN, A RETURN, B RETURN, TRACE IN): 1M Ohm
* Impedance of CV inputs (`FADE` in, `FLIP` in): 100K Ohm
* Range of CV signals (`FADE` in & out, `FLIP` in): 0V-5V
* Output impedance of all outputs: 1K Ohm

#### Repair

All Animation comes with a 2-year warranty from akkusativ.
That means we will repair or replace the pedal for free
during 2 years from the original date or shipment.

This warranty does not cover loss or theft, damage caused by
misuse, abuse, unauthorized modification, improper storage,
or natural disasters. Damage caused by any of the above
circumstances may result in a non-warranty repair fee.

The shipping costs to and from akkusativ are not covered by
the warranty.

After the 2-year period we can repair the product for a fee.

Please send questions and repair requests to `hey@akkusativ.cc`

####  End of Life

We will strive to provide spare parts and repairs for our
products for as long as reasonably possible. Once the
production of All Animation is discontinued, we will publish
all the necessary resources under an open-source license so
that people can repair and modify their devices.

#### Acknowledgements

All Animation would not have been possible without support
and contributions of these people:

* Tracy Goodsmith – for the original proposal of a mixer
  with a flip function and support of the early prototypes
  of what later became All Animation.

* Rebecca Hiles – for all the hard work and support starting
  and running Pedal Markt.

* Cristina Amate from Dochka Films – for every video of All
  Animation and Pedal Markt.

* John Snyder from Electronic Audio Experiments – for
  open-sourcing some of the EAE designs, running an amazing
  Discord community and reviewing the All Animation
  schematic.

* Sascha Hartmann from suchahardman and Christian Maniewski
  – for inspiration, sharing knowledge and electronic
  components :)

Open-source hardware community has been instrumental in what
we do. We owe it to the people that share their knowledge
and designs online. If you are interested in electronics of
music instruments, check them out:

* Berlin Modular community
* Aaron Lanterman
* Moritz Klein
* Steve Demedash
* Matthew Skala
* Synth-DIY mailing list
* Casper Electronics
* Kristian Blåsol

