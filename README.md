# jAmp Percussive (AUv3) manual

Welcome to [jAmp Percussive](https://www.jamp-audio.com/percussive.html), a powerful and innovative drum synthesizer and sequencer designed to elevate your music production experience. Unlike traditional drum machines that rely on pre-recorded samples, jAmp Percussive generates drum sounds using advanced physical modeling techniques, allowing for a highly realistic and dynamic sound palette.
We harness the power of mathematics to create lifelike drum sounds, offering unparalleled control and flexibility. Whether you're producing intricate rhythms or exploring new sonic territories, jAmp Percussive provides the tools you need to craft unique and expressive drum tracks.

Key features include:

  - Physical Modeling Synthesis: Generate drum sounds purely through mathematical models, capturing the nuances and characteristics of real drum instruments.
  - Versatile Sequencer: A built-in sequencer that allows you to create complex and evolving rhythmic patterns with ease.
  - Extensive Sound Shaping: Fine-tune every aspect of your drum sounds with a wide range of parameters and modulation options.

This manual will guide you through the installation, setup, and usage of jAmp Percussive, helping you unlock its full potential and integrate it seamlessly into your music production workflow.

## System requirements

jAmp Percussive is an AUv3 (Audio Unit version 3) plugin that can be used as a stand-alone application on iOS and macOS, or as an audio plugin inside a host application on iOS and macOS. 

Minimal requirements are:
  - iOS 14.0 or later for mobile (iPhone or iPad)
  - macOS 11.0 or later for desktop / laptop

The jAmp Percussive software is distributed via the Apple App store. Click on the App store badge to go to the download location.

[![](images/AppStore.png)](https://apps.apple.com/us/app/jamp-8100/id6450633716)


## Purchase info

Installation of jAmp Percussive is free, but it will run in DEMO mode. This means that every minute jAmp Percussive will output 3 seconds of silence. This allows the user to test the audio plugin in depth before purchasing it.

Purchasing jAmp Percussive is a straightforward and user-friendly process, following the standard steps from the Apple App Store you're likely familiar with. Once the plugin is unlocked, the DEMO mode will be gone, and you can enjoy the full potential.

![](images/purchase.png)

To start the payment process you have to run jAmp Percussive in stand-alone mode. A popup as in the image above should appear. Simply tap or click on "Purchase" and the Apple App Store will guide you through the process.

Note that you should only pay once to unlock the plugin. In case you have a new device, you can get the plugin unlocked by clicking on "Restore". If you go a second time through the payment system, no worries, Apple will notice this and give you the plugin for free.

![](images/purchase_daw.png)

Note that it is not possible to purchase the audio plugin via a third-party host application. If you run jAmp Percussive via for instance GarageBand you will get a message as in the image above. Just start the stand-alone jAmp 8100 application if you want to purchase.


## Synthesizer view

![](images/percussive.png)

The main view of the application contains a navigation bar on top, a bunch of knobs that control the synthesized sounds, a row with some additional settings, and 16 large buttons that will produce a drum sound when hit. 
Let's go over the different buttons and knobs from the bottom of the view to the top.

## 16 large buttons
The large buttons will produce a drum or cymbal sound when they are tapped, or when the corresponding MIDI note is triggered.
There are two types of synthesized sounds available. The 8 top buttons can be used to create membrane based drum sounds, while the bottom 8 buttons are used to create cymbal sounds. 

## MIDI step button
To each button we can assign a MIDI note. Triggering this MIDI note will trigger the corresponding drum or cymbal sound.

## Name id dropdown
Each button can be given a name id. This name id will be used by the sequencer (see later).
The top 8 buttons, corresponding to membrane based drum sounds, can be given one of the following name ids:
  - kick
  - snare
  - tom lo
  - tom hi
  - cowbell

while the bottom 8 buttons, corresponding to cymbal sounds, can be given the following name ids:

  - hihat
  - ride
  - crash

Note that a name id is unique. If a button is given the name id "hihat", then any other "hihat" button will become empty.

## Silence mode
This is a tappable button. When activated, the large buttons will not trigger a sound anymore. This is interesting when one wants to modify the parameters of a drum or cymbal while the sequencer is playing without causing and extra trigger.

## Membrane based drum parameters

### Pitch
Represents the main pitch of the drum sound, in Hertz.

### Decay
Controls the length of resonance of the drum.

### Low pass
A low pass filter that will filter away the higher frequencies.

### Overtone gain
Controls the inharmonicity of the sound by changing the amount of feedback gain in the underlying all-pass filter.

### Overtone pitch
Controls the inharmonicity of the sound by changing the frequency in the underlying all-pass filter.

### Noise pitch
Any noise will first pass through a band pass filter. With this knob the frequency range of this band pass filter can be controlled.

### Noise
Adds filtered white noise to the sound. Mainly used to simulate a snare.

### Pitch bend
When trigger, the drum will start a the initial pitch, but will then bend lower. The amount of pitch bend can be controlled with this knob.

### Mallet
Simulates the usage of soft and hard mallets.

### Velocity
Represents the force of a drum trigger.

### Level
Finetune the gain of this drum.

### Pan
Left or right stereo panning.

## Cymbal based drum parameters

### Pitch
Control the pitch of the cymbal, in steps of half tones. Goes from -24 (or - 2 octaves) to +24 (or + 2 octaves).

### Decay
Controls the length of resonance of the cymbal.

### High pass
A high pass filter that will filter away the lower frequencies.

### Timbre
Changes the overall sound of the cymbal.

### Attack
Sharp attacking sound, or slowly increasing build up of sound.

### Crash delay
This parameter assumes that the "Mallet soft" knob is not fully turned down. The parameter expresses in seconds (0s - 3s) the amount of delay until the cymbal sound "crashes".

### Noise
Controls the amount of filtered white noise.

### Mallet soft
The initial cymbal trigger can be controlled by this knob. It goes from a pop of white noise to a soft oscillating sine pulse, or anything in between.

### Mallet pitch
See previous parameter. This parameter controls the frequency of the soft oscillating sine pulse of the mallet.

### Velocity
Represents the force of a cymbal trigger.

### Level
Finetune the gain of this drum.

### Pan
Left or right stereo panning.

## Navigation bar

On top of the view we have the navigation bar.

### Copy

When in synthesizer view, the copy button will copy the parameters of the current active drum or cymbal.
When in sequencer view, the copy button will copy the current sequencer pattern.

### Paste

When in synthesizer view, the current active drum or cymbal will be replaced by the last copied drum or cymbal.
When in sequencer view, the current active pattern will be replaced by the last copied pattern.

### Presets

Open the presets view. See later for a more detailed description.

### Synth / Sequencer

Switch between the synthesizer view and the sequencer view.

### Play / Stop

Start or stop the sequencer.

### Channels

Open the channels view. See later for a more detailed description.

### Volume knob

Control the overall volume output.

### Light / Dark mode

Change the color scheme of the application.


