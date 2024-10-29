# Wearable Eye Tracker

## Specifications


| _Specification_        | Details                                                                                                 |
|--------------------------|---------------------------------------------------------------------------------------------------------|
| _Sampling Rate_        | Up to 200Hz, default 200Hz                                                                              |
| _Gaze Accuracy_        | 1.8° uncalibrated, 1.3° with offset correction                                                          |
| _Gaze Spatial Resolution_ | 1600x1200 px                                                                                        |
| _PC Interface_         | Neon Companion App, LSL Relay                                                                          |
| _Eye Tracking Technology_ | Real-time neural network                                                                            |
| _Binocular Eye Tracking_ | Yes                                                                                                   |
| _Calibration_          | Calibration-free                                                                                       |
| _Slippage Compensation_ | Slippage invariant. Deep learning powered.                                                            |
| _Scene Camera_         | 1600 x 1200 @ 30Hz                                                                                     |
|                          | H: 1320, V: 810                                                                                        |
| _Eye Cameras_          | 2 x IR eye cameras                                                                                    |
|                          | 192 x 192 @ 200 Hz                                                                                     |
| _IMU_                  | Accelerator, Magnetometer, Gyroscope                                                                   |
| _Microphone_           | Dual microphone                                                                                         |
| _Battery Recording Time_ | Up to 4 hours                                                                                        |
|                          | 25+ hours of recording storage                                                                         |
| _Cable_                | USB-C                                                                                                  |
| _Computing Device_     | Mobile phone: Motorola Edge 40 Pro                                                                     |
| _Real-time Data_       | 2D gaze points in scene camera coordinates at 200 Hz<br>Full head pose, accelerometer and gyro data at 110 Hz<br>IR eye video showing fused eye regions at 200Hz<br>RGB scene video at 30 Hz & Pupilometry data and eye state<br> (Available in Pupil Cloud) Eye position, eye orientation, pupil diameter                                                          |
| _Software_             | Real-time: Neon Companion App                                                                         |
|                          | Post-hoc: Pupil Cloud                                                                                 |

Documentation from Pupil Labs spanning the following topics: Hardware, Data Collection, Pupil Cloud (tool where data is uploaded), Neon Player (tool for playing back and exporting recordings), Real-Time API, Neon XR [Here](https://docs.pupil-labs.com/neon/).

### Adult frames: Just Act Normal

<center>![Adult Frames](img/EyeTracking/1.png)</center>

### Child frames: All Fun and Games (Ages 2 - 8)

<center>![Child Frames](img/EyeTracking/2.png)</center>

## Hardware Setup

### Out of Box Setup for Neon by Pupil Labs

#### Equipment

The following equipment should be included in the Pupil Labs hardware: 

 - Phone to run the wearable eye tracker 
 - Adult frames (that has a space to store the Anker phone)
 - Child frames 
 - Lens kit 

<center>![Boxes](img/EyeTracking/3.png)</center>

You will also need an Anker dongle [Amazon link](https://www.amazon.com/Anker-PowerExpand-Ethernet-Delivery-MacBook/dp/B08C9HZ5YT/). This is not included with Pupil Lab Neon and has been ordered separately.

### Setup Steps

Please follow steps 1 - 9 for the Out of Box instructions to setup the hardware (the wearable glasses)

1. Open the Adult frames and pull out the phone. Turn on the phone.
    - Put a screen protector and a case [link to case] on the phone. Follow the instructions per the screen protection kit: [link to screen protector].
    - Login for phone: 0000 (press 4 times and then press enter - this is not like iPhone where it will go automatically).
    - Use the following Google Account to set-up the phone. This is the Google account used from Neon Companion App and Pupil Labs Cloud:
        - User:
        - PW: 

2. Open the Neon Pamphlet and follow the instructions, which are also written in steps 3 - 4.

3. Install Neon Companion App. Open Google Play Store and search “Neon Companion”.

4. Open Neon Companion App.

5. Plug glasses into the phone.

    - First time you plug in glasses to the phone, it will ask you to allow the Neon Companion to access the Neon Sensor Module and Neon Scene Camera v1. Check the Always open… box, and press OK. <br>
    <img src="../img/EyeTracking/5.png" width='300px'>
    <img src="../img/EyeTracking/6.png" width='300px'>

6. In the Neon Companion App, there are three “tabs” at the bottom.
    - <span style="color:red;">⭘ (red)</span> - Allows you to view recordings.
    - <span style="color:blue;">⭘ (blue)</span> - Recording screen.
    - <span style="color:green;">⭘ (green)</span> - Live Preview. This shows you the view from the glasses.

7. You need to set-up different “Wearers” on the account. Make sure you are in the recording tab (see #6; the blue circle in the image). In the recording tab, go to the bottom left side and click on “Wearer”.
    - Create a wearer called “tester” to run a test recording.
    - Click “Switch Wearer” to create different wearer profiles. Then click the “+ New Wearer” bottom on the bottom right.

8. There needs to be 16 different profiles to accommodate users and participants with varying inter eye distance. Label profiles with just a single number, 50-65. For each profile, click “Adjust” under “Inter Eye Distance” and slide accordingly for the right profile.

9. To switch between wearer profiles, click “Switch Wearer” and then click on the profile you want. Click “Activate” to switch to that profile.

**The hardware is all set-up and ready to start recording!**

## Other Useful Markdown tools:

### Lists

Magnique moenia Herculis Daedalon amnis humus limen, dent cum tenent arbiter:
nulli. Quodque [saepes](http://versatnon.net/pictispartes), quas gestu
alimentaque ulvae postquam **fata sonumque**! Ima **prius**, est ardere summo,
et longa caelum occumbere in dixerat trementi.

#### Unordered Lists

- Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur
  accumsan nibh eu mattis. Vivamus tempus velit eros, porttitor placerat nibh
  lacinia sed. Aenean in finibus diam.

    * Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    * Nam vulputate tincidunt fringilla.
    * Nullam dignissim ultrices urna non auctor.

#### Ordered Lists

1.  Vivamus id mi enim. Integer id turpis sapien. Ut condimentum lobortis
    sagittis. Aliquam purus tellus, faucibus eget urna at, iaculis venenatis
    nulla. Vivamus a pharetra leo.

    1.  Vivamus venenatis porttitor tortor sit amet rutrum. Pellentesque aliquet
        quam enim, eu volutpat urna rutrum a. Nam vehicula nunc mauris, a
        ultricies libero efficitur sed.

    2.  Morbi eget dapibus felis. Vivamus venenatis porttitor tortor sit amet
        rutrum. Pellentesque aliquet quam enim, eu volutpat urna rutrum a.

        1.  Mauris dictum mi lacus
        2.  Ut sit amet placerat ante
        3.  Suspendisse ac eros arcu

#### Definition Lists

`Lorem ipsum dolor sit amet`

:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
    tellus non sem sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`

:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin
    ut eros sed sapien ullamcorper consequat. Nunc ligula ante.

#### Task Lists

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque

### Quotes and Codeblocks

Illos in cupidine avidi. Sub albus claro **nitidum sidere nitentia** irascere,
**silva omnes** terrebit. At Thracum virgae dicta. Auras ferventibus vestis
pervenientia detrahat Baucis, cervice sit mentoque, virtus? Exhortor palmite
poposcit, non aetas stratosque licet Nereides: nacta inpatiens modo nihil deorum
vilibus.

> Nec Procne erit proelia, umeris quem, petunt, **est positis erat**. Per
> dominum tractata. Sustinet quo; virilem cognoscere visa, in imago.

Per visus Lycaoniae cortice. Dixit in despecta umbra. Me tulit flumine imas
dicor aetatis orbam insula ultra sua densetur; ille. Lacteus orbis sed breve,
cara, e tortum tepido ferrum, *dolet* oblivia Hyries equidem saevior usus
**ventis**. Videre motasse, cum tela lyncum, servabunt mansit Arcadiae et
extemplo longa.

Lorem markdownum situsque ut ligari voluptas dummodo moras fata vela lecti
fecere parentis saxea. Primordia quia timentem suadent Heliades, Tonantis aves
nunc tenditur. Latuere volenti solita et inprudens feras. Vidi Lichan at Aeson
et **lapis reluxit**. Viri medio tamen thalami tinguet, clausas, in ambit mille,
ego invadunt Dauno illi!

``` py
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```



### Colored Text (in-line html)

Orange words incoming: <span style="color:orange;">Word up</span>.


### Sub & Superscript

29^th^ H~2~0

### Emojis & Keyboard Keys

:dog: :cat: :) 😀 🫔  💀[find emojis here](https://emojipedia.org/)

++ctrl+alt+del++ [link to all the keys](https://facelessuser.github.io/pymdown-extensions/extensions/keys/#extendingmodifying-key-map-index)


### Marked Text & Footnotes

==Hello Everyone (highlight + bold)==

^^Hello Everyone (highlight)^^

~~Hello Everyone (strikethrough)~~

Footnote 1[^1].

Footnote 2[^2].


[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[^2]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.

### Abbreviations and Tooltips

#### Text with abbreviations

The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium

#### Link with tooltip, inline syntax

[Hover me](https://example.com "I'm a tooltip!")

#### Link with tooltip, reference syntax

[Hover me][example]

  [example]: https://example.com "I'm a tooltip!"
