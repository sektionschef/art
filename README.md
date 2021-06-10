# art portfolio

- [Hello world, hello futuregarden](text/hello_world_hello_futuregarden.md)
- [Data Painting](text/data_painting.md)
- [Projection Painting Prototype](projection_painting_prototype.md)

# Like Converter | Apr 29, 2014

The Like Converter transforms likes earned for a Facebook posting into delicious candy. It is a reward system for social media managers and a source of motivation for your desk.

Video: [![Like Converter](http://img.youtube.com/vi/qcssBxjWfE8/0.jpg)](http://www.youtube.com/watch?v=qcssBxjWfE8 "Like Converter")

The thing itself is built (like the [Twetterhaeuschen](http://digit.alitility.com/tutori-alitility/twetterhauschen/ "Twetterhäuschen")) on a [raspberry pi](http://www.raspberrypi.org/ "raspberry pi"), an [arduino](http://www.arduino.cc/) uno using [node.js](http://nodejs.org/) and [firmata](http://arduino.cc/en/reference/firmata). The source code is on github: <https://github.com/sektionschef/like_converter>

![](uploads/2014/04/P1060877-150x150.jpg)

![The Like Converter sign](uploads/2014/04/P1060880-150x150.jpg)

![](uploads/2014/04/P1060883-150x150.jpg)

![](uploads/2014/04/P1060893-150x150.jpg)

# Die Dübitale Revolution | 2014/03/30

![duebitalanzeige](uploads/2014/03/P1060868.jpg)

Bayrische Großvisionäre haben das Tor zu einer neuen Dimension aufgestoßen. Die "Dübitalanzeige" besteht aus einem Holzbrett, in das durch präzise Bohrungen einzelne Dübel von Hand variabel angeordnet werden können. Je nach Dübelsetzung kann so, eine gewisse geistige Flexibilität vorausgesetzt, eine kurze Botschaft encodiert werden, ohne ein einziges Watt zu verbrauchen.

![Rückseite der Dübitalanzeige](uploads/2014/03/P1060863-150x150.jpg)

![das Düxel](uploads/2014/03/P1060871-150x150.jpg)

![Close Up](uploads/2014/03/P1060868-150x150.jpg)

!["Donkschen" geschrieben auf der Dübitalanzeige](uploads/2014/03/P1060866-150x150.jpg)

Die "Dübitalanzeige" ist der erste große Schritt Richtung dübitaler Ära. Ob das Pixel tatsächlich dem Düxel Platz machen werden muss, wird sich erst in den nächsten Jahren herauskristallisieren.

Die Eckdaten:

- Auflösung: 5x30 Düxel
- Stromverbrauch: 0 kW
- Bildschirmdiagonale: 30''
- Dübcheck & Roe'sche Constraint: 100 Dübel

# Twetterhäuschen | Nov 20, 2013

The Twetterhäuschen is the world's first Wetterhäuschen for visualizing the sentiment of a specific topic on [twitter](http://twitter.com/). It was built on a [raspberry pi](http://www.raspberrypi.org/), a servo controlled by an [arduino uno](http://arduino.cc/), using [node.js](http://nodejs.org/) in combination with [socket.io](http://socket.io/). You can find the code on github to build your own: <https://github.com/sektionschef/twetterhaeuschen>

![](uploads/2013/11/Twetterhaeuschen_01-150x150.jpg)

![](uploads/2013/11/Twetterhaeuschen_02-150x150.jpg)

![](uploads/2013/11/Twetterhaeuschen_03-150x150.jpg)

![](uploads/2013/11/Twetterhaeuschen-Frontend-150x150.png)

## Implementation

1. The Twetterhäuschen has its web form (index.html) to fill a brand or topic of interest
2. The keyword is passed on to the server (app.js) which takes care of the API calls using the [oauth](https://github.com/ciaranj/node-oauth) module. The search is completed with some words to derive a basic level of sentiment, e.g. "love" or "hate"
3. Taking the reach (number of followers) into account, the ratio between good and bad is calculated
4. The arduino sets the servo between the angle of 60 and 130 in order to move the two characters Sepp and Susi out of the Twetterhäuschen.
5. Whereas Sepp represents the dark force, Susi acts as a substitute for ecstacy and elation.

Here is an explanation in German:

<https://www.youtube.com/watch?v=jSNGg0Prsf4> [![Prototype](http://img.youtube.com/vi/jSNGg0Prsf4/0.jpg)](http://www.youtube.com/watch?v=jSNGg0Prsf4)

# Paintings

![Nagano - Acrylic on canvas, 160x100cm](uploads/2013/05/nagano_ub.jpg "Nagano - Acrylic on canvas, 160x100cm")

![Wühlmaus](uploads/2013/03/P1020296.jpg "Wühlmaus")

![Skeleton](uploads/2013/03/P1020294.jpg "Skeleton")

![Staro](uploads/2013/03/P1020293.jpg "Staro")

![Magazino](uploads/2013/03/P1020291.jpg "Magazino")

![Dochboden](uploads/2013/03/P1020289.jpg "Dochboden")

![Schuachschochtl 1](uploads/2013/03/P1020285.jpg "Schuachschochtl 1") ![Schuachschochtl 2](uploads/2013/03/P1020282.jpg "Schuachschochtl 2") ![Schuachschochtl 3](uploads/2013/03/P1020287.jpg "Schuachschochtl 3")

# Animation in the command line - ./animation.sh | Jan 29, 2012

## Introduction

After finding out how much one can do with [ffmpeg](http://www.ffmpeg.org/ "http://www.ffmpeg.org/")... I thought it would be the perfect tool for creating my abstract stop-motion animation I dreamed of for years. What I wanted to realize was simple: combining scenes of a series of high resolution photographs, including images of paintings and digitally edited material with various lengths, framerates exactly timed to a soundtrack.

Ffmpeg is a powerful tool to convert audio and video files (among other things). It allows to define many parameter and enables batch processing videos. What it does not provide is a graphical interface for cutting and editing the files. So I learned some BASH and wrote a script to achieve my goals. All I am working with is a directory where the scenes are stored, a text file which defines the time, the framerate and the position of the individual scenes and the final output video.

The advantages are that I exactly get what I want and that I learned a lot. It's the simple, clear way of editing the project as well as the separation of media and the concept that I really like about this method. The disadvantages are the time until the whole video is rendered - it takes approximately an hour until the HD version of the video is rendered. For this project, I still think that this approach is in fact easier than working with a large-scale video editing software.

Here is the final result: <https://vimeo.com/18348528>

The video itself is my personal art project. It features some visual, experimental ideas. It was done on the basis of my own photos and paintings/drawings and simply deals with "seeing things" as well as how to achieve a flat picture from a real world 3d image. I am messing with colours, perspective, light and movement. In the beginning everything is about an impression of movement using still images. Additionally, the animations of signs and graffiti support the topic of movement and are used to separate certain blocks of scenes. Then, similar geometric forms found on the streets are shown. The exact alignment of the photos emphasizes the similarities of the objects. The next scenes of the animation deal with colours and colour differences that were generated by manipulating the contrast.

The following animations should show a certain difficulty of perceiving depth in the images. The next images continue this idea and visualize the transformation from the three dimensional reality to the flat, two dimensional image of that reality. The animations featuring the rectangles of black tape invert this process by actually projecting a flat rectangle back in the real space. The rectangle is solely visible from the perspective of the camera.

![](uploads/2012/01/equip-150x150.jpg)

![](uploads/2012/01/equip02-150x150.jpg)

![](uploads/2012/01/equip03-150x150.jpg)

Similarly, the images feature how space, a white wall with corners, are reduced to different shades of white. The change of perspective creates different minimalist images. In the paintings the topics are applied practically. It is moreover interesting to see, how these evolve. The wood frame in the end acts as a summary by showing the same object in different states: during the different colours of daylight, with a moving light source and the wood frame moving itself.

I chose the song _Mouthpiece_ by the band [Shellac](http://www.touchandgorecords.com/bands/band.php?id=22 "http://www.touchandgorecords.com/bands/band.php?id=22") as a soundtrack. The song is vital to the film providing the rhythm of the transitions and it is a brilliant song.

## Manipulating Images

Most of the images need some form of editing or need to be arranged to achieve a proper overlay in order to focus on specific differences in the images and erase the unwanted differences. Some changes are created just by manipulating pictures.

For image manipulation I use the [Gimp](http://www.gimp.org/ "http://www.gimp.org/"). Each scene's frame is one layer and the whole scene can be saved with all layers in the .xcf format. The task of aligning the layers is easy with the right script, [exact aligner](http://registry.gimp.org/node/18961 "http://registry.gimp.org/node/18961"). Just draw a line on two layers to define two identical parts in both images. After running the script from the menu the second line is fitted to the first line - hard to explain, easy to grasp. Usually I crop the canvas a little (in the aspect ratio of 4:3).

Then another wonderful [script](http://registry.gimp.org/node/15617 "http://registry.gimp.org/node/15617") enables me to export all layers as separate .jpg files (I only needed to edit the default filename in the script itself from .png to .jpg). I also changed the Gimp's default .jpg quality settings. The result is a couple of .jpgs in your home folder with the scene's filename and a continuous frame number. The scripts take care of the rest.

## First Attempt

The first task for me was to define a workflow what tasks need to be done, in what sequence, how to organize the files and how to change the parameters in a convenient way. The 3 basic operations I wanted are:

- Create a new scene with a set of images
- Edit parameters of existing scenes
- Edit parameters of all scenes at once

The basic command for ffmpeg to render a video based on images is something like:

`ffmpeg -loop_input -f image2 -r <FRAMERATE_SCENE> -i "input_frame_%04d.jpg" -vframes <LENGTH> "output.avi"`

As a result, the basic parameters are the **framerate** of the scene, its **length** and the **input filename**, which is given as _%04d_. This means that the format of the number is 4 digits, 0001-9999 ([helpful link](http://spielwiese.la-evento.com/hokuspokus/ "http://spielwiese.la-evento.com/hokuspokus/")). Furthermore, the [ffmpeg faq](http://www.ffmpeg.org/faq.html "http://www.ffmpeg.org/faq.html") points out that .avi files can be concatenated using the _cat_ command - merging the files with the result of one single video. However, the cat command does not know in which sequence to merge the files. For the correct order of all scenes a **numbering** is needed, which I called „rank", and this should become part of the filename. The _cat_ command starts with the first number and continues until the last frame. In sum, the framerate, the length and the rank are the parameters which determine the editing of the video file. These parameters should be easily changeable. The only thing which should be invariable is the scene's name.

For easing my task and keeping an overview I wrote these parameters in a separate .csv file (comma separated file). There I can reschedule the scenes, the framerates and the length at once. For rescheduling, sorting, calculating and changing the scenes the .csv file can be imported in open office spreadsheet. The cutlist is in the form of:

```
RANK;SCENE;FRAMERATE;LENGTH
0001;abdeckungen;4;30;
0002;radl;4;50;
```

My first version script (you can find in the [appendix](http://tutori.alitility.com/doku.php?id=ubuntu:animation_in_the_command_line#one_after_the_other_script "ubuntu:animation_in_the_command_line")) begins by asking the only parameter a scene name from the user. The input is then checked if it already exists or not, which determines the subsequent operations. If the input is _all_ all scenes are rendered according to the parameters of the cutlist.

The cutlist file is read for the needed parameters or if the scene is not yet existing these are entered directly to the terminal and written to the cutlist. For new scenes a directory is made, the frames transferred to this directory, resized to the wished size using imagemagick, renamed to include the scenes' rank and rendered. If the rank has changed the filename of all videos is renamed and the scene is rendered according to the new parameters.

In the final block which is run in any case the filenames of all video outputs is checked against the cutlist.csv in order to remove obsolete files, which would mess up the _cat_ command. Then all videos are merged by _cat_ in the sequence of the rank and the soundtrack is added by ffmpeg. Que bello!

## Picture in Picture Animation

Soon after finishing my first script and celebrating my success I realized that the end result became a victim of the worst enemy art films have to face - boredom. The scenes were cut one after the other and the proper mojo was missing. What I actually wanted was displaying several scenes at once (picture in picture) in order to emphasize a relationship among them. In [imagemagick](http://www.imagemagick.org/script/index.php "http://www.imagemagick.org/script/index.php") I found a way of realizing what I wanted using layers. The basic command for this is:

```
for i in {1..5}
do
convert -size 1440x1080 xc:black "a_*$i.jpg" -geometry 700x525+383+6 -composite "b_*$i.jpg" -geometry 700x525+13+546 -composite "c_*$i.jpg" -geometry 700x525+728+546 -composite "output_`printf "%04d" $i`.jpg"
done
```

I started all over again, this time letting imagemagick render the frames by arranging several pictures into one. The frames need to be processed individually before I can render a scene. As a consequence every single frame of the final video is rendered in imagemagick and then processed by ffmpeg. The scenes are layers on a 1440×1080 canvas in black color. The output is a frame in the format ffmpeg is able to use. Having each frame rendered takes quite some time! Still, the quality is amazing.

On the basis of this command I came up with a new workflow consisting of 3 separate scripts:

- rendering the whole video or just parts of it (by defining a frame range in the terminal)
- a preview script, for monitoring single scenes (use export of gimp; defining the framerate in the terminal)
- importing a scene in my cutlist

Like in the first script I use a .csv file for the parameters, which is a little bit expanded now. The difference compared to the cutlist of my first script is a column for the PIP parameter, a category column and frank instead of rank and the endfrank instead of length. The PIP parameter defines where the scene is placed on the canvas. The category just helps me to organize and filter the scenes while editing the .csv file directly but has no impact on the process itself. The biggest difference is frank, the frame the scene appears for the first time in the final video. On the contrast, the rank of the first script was just ordinal. The endfrank is the last frame in the video the scene is shown - this quite helps with the timing when cutting the scenes. The cutlist looks like this:

```
FRANK;SCENE;FRAMERATE;ENDFRANK;PIP(wxh+w_o+h_o);CATEGORY 50;emergencydahoam;7;600;900x675+980+365;animation_bewegung 275;stiegeberlin;5;650;900x675+40+40;animation_bewegung 700;ubahnstill;8;786;1440x1080+240+0;animation 787;ubahn;8;990;1440x1080+240+0;animation 1000;benettonromdoppelt;5;1195;900x675+980+202;bewegung 1005;benettonrom;5;1200;900x675+40+202;bewegung 1211;kabelsalatrom;5;1471;640x480+1120+560;bewegung 1226;gradeskabelrom;5;1486;640x480+1120+40;bewegung 1253;kabelangelbrom;5;1501;640x480+160+560;bewegung 1268;hinundherrom;5;1522;640x480+160+40;bewegung 1542;abdeckungen;4;1738;900x675+980+365;gleicheformen 1644;gitterfenster;4;1859;900x675+40+40;gleicheformen 1738;malewitschrom;4;1968;900x675+980+40;gleicheformen 1860;fensterneubaugasse;4;2068;900x675+40+365;gleicheformen 2088;dreckradrom;8;2281;900x675+980+202;animation 2088;dreckbamrom;8;2281;900x675+40+202;animation 2302;farbengelbblinkybill;4;2550;900x675+980+202;farbe_gelb 2312;farbengelbvierkant;4;2595;900x675+40+202;farbe_gelb 2550;farbengraumauer;3;2833;900x675+980+202;farbe_grau 2595;farbengraucanvas;4;2880;900x675+40+202;farbe_grau 2833;farbenalles;5;3040;900x675+980+202;farbe 2880;gumpsn;2;3069;900x675+40+202;farbe 3093;radl;8;3274;1440x1080+240+0;animation_bewegung 3290;wienfluss;10;3506;900x675+1200+202;tiefe 3300;meyerrom;10;3536;900x675+240+202;tiefe 3521;andreahandrom;10;3780;900x675+980+202;tiefe 3550;leibalberlin;5;3780;900x675+40+202;animation_tiefe 3794;leopolda;5;4003;640x480+640+40;3d 3824;leopoldb;5;4003;640x480+160+560;3d 3854;leopoldc;5;4003;640x480+1120+560;3d 4014;dreieckroma;5;4223;640x480+640+40;3d 4044;dreieckromb;5;4223;640x480+160+560;3d 4074;dreieckromc;5;4223;640x480+1120+560;3d 4234;balkenbaerberlina;5;4453;640x480+640+40;3d 4264;balkenbaerberlinb;5;4453;640x480+160+560;3d 4294;balkenbaerberlinc;5;4453;640x480+1120+560;3d 4474;oelschranka;2;4570;1440x1080+240+0;perspektive 4570;oelschrankb;5;4860;1440x1080+240+0;perspektive 4884;rechteckb;2;5028;640x480+1120+40;perspektive 4884;rechteckd;2;5028;640x480+1120+560;perspektive 4884;rechtecka;2;5028;640x480+160+40;perspektive 4884;rechteckc;2;5028;640x480+160+560;perspektive 5028;rechteckabcddoppelt;5;5293;640x480+1120+40;perspektive 5028;rechteckabcdvierfach;5;5293;640x480+1120+560;perspektive 5028;rechteckabcd;5;5293;640x480+160+40;perspektive 5028;rechteckabcddreifach;5;5293;640x480+160+560;perspektive 5320;powerhouseberlin;6;5590;900x675+40+40;2d 5320;vogelberlin;6;5590;900x675+980+365;2d 5590;jedermannberlin;4;5840;900x675+40+365;2d 5590;tucholsky;5;5840;900x675+980+40;2d 5886;malereiberlina;2;6376;640x480+640+40;malerei 5966;malereiberlinc;2;6376;640x480+1120+560;malerei 6046;malereiberlinb;2;6376;640x480+160+560;malerei 6376;malereiberlinbstill;5;6511;640x480+160+560;malerei 6376;malereiberlincstill;5;6554;640x480+1120+560;malerei 6376;malereiberlinastill;5;6602;640x480+640+40;malerei 6659;blumenkastldrehenstill;5;6788;640x480+160+560;alles 6716;blumenkastllichtstill;5;6788;640x480+640+40;alles 6770;blumenkastllichtdrehenstill;5;6788;640x480+1120+560;alles 6788;blumenkastldrehenpreludium;7;6806;640x480+160+560;alles 6788;blumenkastllicht;10;7023;640x480+640+40;alles 6788;blumenkastllichtdrehen;7;7023;640x480+1120+560;alles 6806;blumenkastldrehen;7;7023;640x480+160+560;alles
```

I calculated some standard picture in picture positions for arranging the scenes:

![animation_04b](uploads/2012/01/animation_04b.png)![animation_03b](uploads/2012/01/animation_03b.png)![animation_04](uploads/2012/01/animation_04.png)![animation_03](uploads/2012/01/animation_03.png)![animation_02b](uploads/2012/01/animation_02b.png)![animation_02](uploads/2012/01/animation_02.png)

here is a flowchart: ![flowchart_animation](uploads/2012/01/flowchart_animation.png)

### Preview

Gimp owns an animation preview function (filters > animation > playback) but I don't really like it. My images have a higher resolution and must be rescaled before viewing the animation and changing the framerate is a pain in the ass. I wrote a script which does the same thing only a bit more convenient. At the same time, it is the first step before importing a scene in my project.

The framerate is set in the terminal as $1 otherwise a default value of 5 is used. The other variables for this little script is the image size and the bitrate of the preview video. After the images have been exported from gimp they are moved from the home directory to the preview directory, resized and renamed. If no images are in the home directory the script processes those of the preview directory so I can experiment with different framerates quickly. The preview directory is emptied if new images have been exported to the home directory. The video itself is created by the basic ffmpeg command for these situations. That's it basically!

```bash
#! /bin/bash

FRAMERATE=$1
# can be set as part of the command

BITRATE=10000k
LENGTH=100

PREVIEW_DIRECTORY=06_preview
SIZE=x1080

if [ -z "$FRAMERATE" ]
then
   FRAMERATE="5"
fi
# sets a default value for framerate

if [ -z "`ls ~ | grep "_*.jpg"`" ]

then
echo "+++++++++ already exists ++++++"

else
#clean house
rm -f $PREVIEW_DIRECTORY/*.jpg

echo "+++++++++ Copy frames to preview directory ++++++++++"
mv ~/*.jpg $PREVIEW_DIRECTORY

echo "+++++++++ Resize frames ++++++++++"
mogrify -resize $SIZE $PREVIEW_DIRECTORY/frame_*.jpg

fi

echo "+++++++++++++ Render $SCENE ++++++++++++"
ffmpeg -y -loop_input -r $FRAMERATE -f image2 -i "$PREVIEW_DIRECTORY/frame_%04d.jpg" -vframes $LENGTH -b $BITRATE -r 25 preview.avi

exit
```

## Importing new scene in project

In case I liked the preview, it is included in the cutlist and therefore part of the project. The following script accomplishes this task without any woes. It asks for the details and parameters in the terminal and writes them into a new line of the cutlist. Before that the contents of the cutlist are shown in order to have some sort of orientation where to put it. For security reasons, the script also checks if the scene's name is already existing. Additionally, a new directory (named after the scene name) is created, the images are moved there and are also renamed properly by including the scene name.

```bash
#! /bin/bash

###########################################################
CUTLIST=cutlist_hobo.csv
PREVIEW_DIRECTORY=06_preview

###########################################################

echo ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
echo "Please enter the SCENE's name:"
echo ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
read INPUT_SCENE

# check if input scene is unique
if [ -z "`grep ";${INPUT_SCENE};" $CUTLIST`" ]

then

cat $CUTLIST

echo +++++++++ "Define parameters" ++++++++++
echo "Please enter its FRANK:"
read INPUT_FRANK
echo "Please enter the framerate:"
read INPUT_FRAMERATE
echo "Please enter the last frame's number:"
read INPUT_LENGTH
echo "Please enter the PIP parameters (wxh+w_o+h_o):"
read INPUT_PIP

echo +++++++++ "Create directory $INPUT_SCENE" ++++++++++
mkdir -p 02_scenes/$INPUT_SCENE

echo +++++++++ "Copy frames to newly created directory" ++++++++++
mv $PREVIEW_DIRECTORY/*.jpg 02_scenes/$INPUT_SCENE

echo +++++++++++++ "Rename by adding the scene's name" ++++++++++++
for FILE in 02_scenes/$INPUT_SCENE/frame_*.jpg ;
do
NEWFILE=`echo $FILE | sed "s/frame/$INPUT_SCENE\_frame/g"` ;
mv "$FILE" $NEWFILE ;
done

echo +++++++++++++ "Write variables to cutlist" ++++++++++++
echo "$INPUT_FRANK;$INPUT_SCENE;$INPUT_FRAMERATE;$INPUT_LENGTH;$INPUT_PIP;" >> $CUTLIST

else
read -p "+++++++++++++ Name of scene is already existing ++++++++++++"

fi

exit
```

## Script for rendering the PIP video

### Render framerate and length

The first part covers the conversion of my images in frames for the video, i.e. the images are brought to the correct framerate and length. Because of arranging the scenes frame-by-frame, I have to do this by myself and cannot simply tell ffmpeg to deal with it like in the first script. But let's start with one thing after the other.

First, the variables are defined. It is possible to define a frame range when running the script in the terminal, in which the script is processed. For instance, frame 500 to 1000\. The default value is frame 1 to frame 7270 which is approximately the end of the soundtrack. The overall framerate I chose is 25 seconds per frame following the PAL standard. The canvas size is 1920×1080 and the bitrate for the final movie is also defined by a variable. Once the video is finished I might render it with a higher bitrate.

Next, each scene's parameters are read from the cutlist: the frank, the length, the framerate and the scene per PIP frame. Additionally, the number of the original frames in the directory is counted. The length is derived by the difference between frank and the end frame of the scene. For matching the strings of scene names, I use the delimiter ";", otherwise equal parts of names would be found as well (looking for "deck" finds scene name "deck" but also "abdeckungen"). For debugging, the scripts prints the parameters it finds for each scene.

Now, the mess begins. For clarification, I'll use an example. The basic parameters we need is the length _l_, how long the scene is displayed i.e. how many frames, and the framerate _r_, how fast the images change. Furthermore, we also need to know how many images the original animation consists of _o_.

```
r... 10
l... 600
o... 4 (A,B,C,D)
```

Mind the difference between frame and image. Image for me is one of the pictures made for the scene, in the example A-D. Frame for me is one of the pictures the final video consists of, 25 frames per second in my case.

The image has to be copied to a certain amount in order to reach the framerate defined in the cutlist. This amount is calculated by the overall framerate divided by the desired framerate, 25/10 = 2.5\. Mind that Bash gives only the integer output of 2\. Neglecting the 0.5 (dealing with this later), the image has to be copied once. Afterwards, the second image B has to be copied as well as the remaining images of the animation (C,D). This procedure has to be done until the end frame of 600 is reached. I think this is what my math teacher used to call series and rows.

I realized this function by implementing two loops, the outer loop covering the length count and the inner loop carrying out the framerate copy. The inner loop, called framerate_boost, is starting at 1 and ends at the 25/2 increasing by 1\. Once this loop is done for an image it falls back to the outer loop, the length_boost, starting at 0 ending at 600 - 1\. The increment of the length_boost must be also 25/2\. In the examples the length_boost has the following values: 0,2,4,6... and 0,5,10,15... respectively. The loop itself has no function but enables to copy the different images one after the other until the last frame of the scene.

The animation would look like this:

<div>
  <table>
  <tbody><tr><th>Frame</th><th>Image</th><th>Framerate Loop</th><th>Length Loop</th></tr><tr><td>1</td><td>A</td><td>1st frame_boost</td><td rowspan="2">1st length_boost</td></tr><tr><td>2</td><td>A</td><td>2nd frame_boost</td></tr><tr><td>3</td><td>B</td><td>1st frame_boost</td><td rowspan="2">2nd length_boost</td></tr><tr><td>4</td><td>B</td><td>2nd frame_boost</td></tr><tr><td>5</td><td>C</td><td>1st frame_boost</td><td rowspan="2">3rd length_boost</td></tr><tr><td>6</td><td>C</td><td>2nd frame_boost</td></tr><tr><td>7</td><td>D</td><td>1st frame_boost</td><td rowspan="2">4th length_boost</td></tr><tr><td>8</td><td>D</td><td>2nd frame_boost</td></tr><tr><td>9</td><td>A</td><td>1st frame_boost</td><td rowspan="2">5th length_boost</td></tr><tr><td>10</td><td>A</td><td>2nd frame_boost</td></tr><tr><td>11</td><td>B</td><td>1st frame_boost</td><td rowspan="2">6th length_boost</td></tr><tr><td>..</td><td>..</td><td>..</td></tr><tr><td>600</td><td>D</td><td>2nd frame_boost</td><td>300th length_boost</td></tr></tbody>
</table>
</div>

for r... 5

<div>
  <table>
  <tbody><tr><th>Frame</th><th>Image</th><th>Framerate Loop</th><th>Length Loop</th></tr><tr><td>1</td><td>A</td><td>1st frame_boost</td><td rowspan="5">1st length_boost</td></tr><tr><td>2</td><td>A</td><td>2nd frame_boost</td></tr><tr><td>3</td><td>A</td><td>3rd frame_boost</td></tr><tr><td>4</td><td>A</td><td>4th frame_boost</td></tr><tr><td>5</td><td>A</td><td>5th frame_boost</td></tr><tr><td>6</td><td>B</td><td>1st frame_boost</td><td rowspan="5">2nd length_boost</td></tr><tr><td>7</td><td>B</td><td>2nd frame_boost</td></tr><tr><td>8</td><td>B</td><td>3rd frame_boost</td></tr><tr><td>9</td><td>B</td><td>4th frame_boost</td></tr><tr><td>10</td><td>B</td><td>5th frame_boost</td></tr><tr><td>11</td><td>C</td><td>1st frame_boost</td><td rowspan="2">3rd length_boost</td></tr><tr><td>..</td><td>..</td><td>..</td></tr><tr><td>600</td><td>D</td><td>5th frame_boost</td><td>12th length_boost</td></tr></tbody>
</table>
</div>

the end result could look like this (although it has an infinite loop):

with r = 10 ![animation_ball](uploads/2012/01/animation_ball.gif) with r = 5 ![animation_ball_slow](uploads/2012/01/animation_ball_slow.gif)

Now, the problem arises that the copy command of the inner loop has to address the correct filenames of the images A-D. For the first frames A, for the next couple of frames B and so on. No wildcards can be used. (otherwise the error notification of _directory file not existing_ shows up). The filenames of the images are in the form of 0001,0002... Therefore, a frame counter is needed which provides the correct number in the images' filenames. This counter has to be defined in the outer loop, because here the image is selected. I'll use the example from before with r = 10 frames per second.

The length_boost counter, with the increment of 25/10, overall framerate divided by desired framerate, can to rearranged by 0_25/10, 1_25/10, 2_25/10,... n_25/10\. My solution was then to divide the actual length_boost by (25/r + 1), which provides a series of consecutive numbers 1,2,3,..n. This variable can be used to address the images by their filename. Unfortunately, this is not the end of the story. There is the problem that those frame numbers exceeding the number of images (A,B,C,D) are not existing, the numbers >4\. When the last image D or 0004 was used the process should start from the beginning, image A or 0001\. The 9th frame should be sourced from picture A.

<div>
  <table>
  <tbody><tr><th>Length_boost counter</th><th>Image Number</th><th>Increment</th><th>Rearranging</th><th>$COUNTER</th></tr><tr><td>0</td><td>0001</td><td>+2</td><td>0<em>2</em></td><td>0/2+1=1</td></tr><tr><td>2</td><td>0002</td><td>+2</td><td>12</td><td>2/2+1=2</td></tr><tr><td>4</td><td>0003</td><td>+2</td><td>2<em>2</em></td><td>4/2+1=3</td></tr><tr><td>6</td><td>0004</td><td>+2</td><td>32</td><td>6/2+1=4</td></tr></tbody>
</table>
</div>

I used to overcome this problem with the formula: _$counter-o_$counter/o_. This formula checks how often the original_frame number is present in the counter. Later (when converting time into numbers of frames), I discovered that there is a built in function, called [remainder](http://www.computing.net/answers/unix/remainder-operator/6820.html "http://www.computing.net/answers/unix/remainder-operator/6820.html") or modulo_% for bash. Took me a while to fully understand it: 5/2=2 and 5%2=1\. The remainder is the left over after a division of two integers ([wikipedia](http://en.wikipedia.org/wiki/Remainder "http://en.wikipedia.org/wiki/Remainder")). By using the remainder like this _$counter%o_ the resulting series stays inside the limit of the number of images. Basically, this is the same thing as using as the formular above. One problem still remains! For making things even more complicated this does not work for multiples of the number of animation images _o_, as _4%4_ equals _0_. A single if condition is able to correct this issue. puh!

<div>
  <table>
  <tbody><tr><th>Length_boost counter</th><th>$COUNTER</th><th>$COUNTER_RESTART</th></tr><tr><td>0</td><td>0/2+1=1</td><td>1%4=1</td></tr><tr><td>2</td><td>2/2+1=2</td><td>2%4=2</td></tr><tr><td>4</td><td>4/2+1=3</td><td>3%4=3</td></tr><tr><td>6</td><td>6/2+1=4</td><td>4%4=0, if condition =4</td></tr><tr><td>8</td><td>8/2+1=5</td><td>5%4=1</td></tr><tr><td>10</td><td>10/2+1=6</td><td>6%4=2</td></tr><tr><td>12</td><td>12/2+1=7</td><td>7%4=3</td></tr><tr><td>14</td><td>14/2+1=8</td><td>8%4=0, if condition =4</td></tr></tbody>
</table>
</div>

Additionally, the copy command must include the scenename and the frame count (the number of the frame it appears in the final video) in the filenames of the frames. The frame count is realized by summing up the loop counters length_boost, framerate_boost. This is the reason why the length_boost starts at zero and not at 1\. In order to additionally have the actual frame of the final video the frank -1 is also included. The final result is that each scene is properly positioned due to the frame number in the filename and each scene has the correct value of iteration. In the next step this material will be put together in the correct way, frame by frame.

### Render pip frames

The next step is to read out the PIP positions from the cutlist for every scene. On the basis of this information the single frames are created. A temporary directory saves the PIP informations and frames before they are rendered in the next section of the script. This temp file is emptied every run and the frames are newly created.

For every frame a text file is created in which the scene's PIP position is written. The PIP position is in the form of expanding the imagemagick command to process several layers. This means the txt file consists of the parameters which are to be included in the imagemagick command to create the layer for each frame. If the frame does not feature any scenes the text file is empty. An example for a scene's command in a .txt file would be:

`<filename> -geometry <PIP position> -composite`

Echo adds these command parts for every scene without using a new line. This is important for including the .txt file into the imagemagick command.

I added the printf command for the creation of the filenames of the final frames because ffmpeg needs them in the form of 0001\. I also added the type True Color because otherwise ffmpeg would return the video in grayscale if the first frames were just black screen. Additionally, ffmpeg is processing the images if the file starts from frame 0001 and not 0520.

### Render Video

The last step is the ffmpeg command for converting images into video. Before we can do that we have to take care of the starting points. Since the rendering takes a lot of time, the script should enable me to see the changes of parameters and timings right away by just presenting a short range of frames, for instance from frame 2000 until frame 2180\. In this regard, the soundtrack is especially important, so we need to convert the starting frame into the song's position or to be more precisely time in the form of hh:mm:ss.xxx (hours:minutes:seconds.milliseconds). This task can be done using the remainder we already learned (well, I learned about it here and it took quite some time). Anyway, we can skip the hours because we won't reach these dimensions, the length of my video is about 4 minutes. For the rest one has to know that one second features 25 frames (of course only if the framerate of the final video is 25!). A minute, therefore, features 25_60 frames and one millisecond features 1/40 frames (1000ms=1s=25frames). The starting frame is first checked against the minutes (start_frame/(25_60)). The rest, the remainder %(25_60), is used to derive the seconds /25 and finally the remaining frames are formatted to milliseconds by %(25_60)%25*40\. This ensures that the timing of the selection (starting at a certain frame and ending at a certain frame) corresponds exactly to timing of the sound at this position.

The ffmpeg command is then only the simple conversion of my rendered PIP frames to a video file. No special parameters are relevant here. The start and end frame determine the length of the video and the calculated delay of the soundtrack is included.

### Important notes

The script's concept is based on the rule that a scene name is only given once... repeating a scene must result in a new scene name. The names of the scenes should have no underscores either as it is used as a delimiter in the filenames. Total confusion or apocalypse would be the logical consequence.

The _0_ after the wildcard _*_ in the cp command is necessary because otherwise a 0011 and 0001 cannot be distinguished. It is however necessary as the script I use to export gimp's layers as .jpg files uses leading zeros (e.g. 00123). This approach might be a little bit risky as one digit is missing (0150 is found; 1150 is not found). my frame numbers are not that high so I do not run into problems with this solution... at least not yet.

The framerate and the actual the framerate of the script are different due to the fact that the calculation _overall_framerate/desired_framerate_(25/10) does not necessarily lead to integer numbers. Bash, luckily, gives only the integer numbers, in our example 2\. This is not necessarily a bad thing, because the correct framerate would extend the length of the scene. Having a fixed length of a scene is, however, really important. Furthermore, the final video should have 25 frames per second and therefore the framerate should be a multiple of 25.

Ffmpeg again needs leading zeros for its frame numbers, so conversion from normal numbers (e.g. 123). the printf command is the right tool for this, in the other direction a 0* does the trick, outlined above.

The PIP script is using cut (combined with _sed '1d'_ for dropping first row) instead of csvtool which I used in my first script. Basically, it provides the same task for me without installing an additional package.

Some of the names I use in my script sound stupid... I just named it to something that came to my mind ( the name westling for instance originates from the Swedish royals, who married when I was writing this script). But there are many comments for clarifying everything.

### The script

```bash
#! /bin/bash

##################### Variables ###########################
START_FRAME=$1
END_FRAME=$2
OVERALL_ASPECT_RATIO=1920x1080
OVERALL_FRAMERATE=25
# important for calculating the number of needed frames of the individual framerate

# default values for length
if [ -z "$START_FRAME" ]
then
   START_FRAME="1"
fi
if [ -z "$END_FRAME" ]
then
   END_FRAME="7150"
fi

#directories and files
CUTLIST=cutlist_hobo.csv
WESTLING=03_westling
TEMP=04_temp

###################################################

echo "##################### Render Framerate and Length ########################"

# clean the house
rm -f $WESTLING/*.jpg

#### Loop for scene name reading all necessary parameters in cutlist ####
for SCENE_NAME in `sed '1d' $CUTLIST | cut -d ';' -f 2 -`
# sed '1d' eliminates the first row of column headers, cut reads the columns using the delimiter ";"
do

# the; around the scene name prevents confusion of strings
FRANK ()
{
grep ";$SCENE_NAME;" $CUTLIST | cut -d ';' -f 1 -
}
LENGTH ()
{
echo $(( `grep ";$SCENE_NAME;" $CUTLIST | cut -d ';' -f 4 -` - `FRANK` ))
}
# length should be a multiple of original_frames and framerate!
# length is now in absolute frame numbers of the final video
FRAMERATE ()
{
grep ";$SCENE_NAME;" $CUTLIST | cut -d ';' -f 3 -
}
SCENE_PIP_PER_FRAME () { grep ";$SCENE_NAME_PER_FRAME;" $CUTLIST | cut -d ';' -f 5; }
# this function matches the scenename from the filename with the one in the cutlist and reads the pip parameter accordingly.
ORIGINAL_FRAMES()
{
ls 02_scenes/"$SCENE_NAME"/"$SCENE_NAME"_frame_*.jpg | wc -w #no idea why -l does not work!!!
}
# counts the number of original frames of the scene

# if the scene is not in the defined frame range, its loop is skipped
if ((`FRANK` < "$START_FRAME"))
    then
    continue
fi

if ((`FRANK` > "$END_FRAME"))
    then
    break
fi

#echo parameters for debugging
echo "++++ Scene Name: "$SCENE_NAME" ++++"
echo "Frank: `FRANK`"
echo "Length: `LENGTH`"
echo "Framerate: `FRAMERATE`"
echo "Original Frames: `ORIGINAL_FRAMES`"
echo "-------------------------------------------------------"

#### first loop - Length Boost ####
for ((LENGTH_BOOST = 0;LENGTH_BOOST <= $((`LENGTH` - 1));LENGTH_BOOST = LENGTH_BOOST + $(($OVERALL_FRAMERATE/`FRAMERATE`)))) do
# "0" because added to the framerate_boost loop .. length of scene .. increment is derived
# length minus one because it starts from 0

COUNTER=$(($LENGTH_BOOST / ($OVERALL_FRAMERATE / `FRAMERATE`)+1))
# counts which frame is copied, important for the cp command
# does not restart
# no idea why brackets are necessary!!

COUNTER_RESTART=$(($COUNTER%`ORIGINAL_FRAMES`))
# accomplishes the restart with the remainder

#### second loop - Framerate Boost ####
for ((FRAMERATE_BOOST = 1;FRAMERATE_BOOST <= $(($OVERALL_FRAMERATE/`FRAMERATE`));FRAMERATE_BOOST++)) do

if [ $COUNTER_RESTART = 0 ]; then
cp 02_scenes/$SCENE_NAME/${SCENE_NAME}_*0`ORIGINAL_FRAMES`.jpg $WESTLING/${SCENE_NAME}_$(($LENGTH_BOOST+$FRAMERATE_BOOST+`FRANK`-1)).jpg
else
cp 02_scenes/$SCENE_NAME/${SCENE_NAME}_*0${COUNTER_RESTART}.jpg $WESTLING/${SCENE_NAME}_$(($LENGTH_BOOST+$FRAMERATE_BOOST+`FRANK`-1)).jpg
fi
# the 0 of the cp command after the wildcard is risky, but not more than 2 digits
# additionally to the length und framerate boost the actual position (framenumber), i called it frank, of the final video is added, the final position is written in the filename for the next stage.

done # end FRAMERATE_BOOST
done # end LENGTH_BOOST

done # end loop SCENE_NAME

echo "########################### Render PIP Frames ##############################"
# find scenename and then read pip parameters for each frame

# clean the house
rm -f $TEMP/*.txt # -f prevents errors of already empty directories
rm -f $TEMP/*.jpg

for ((i=$START_FRAME;i<=$END_FRAME;i++))
do
echo -n "" >> "$TEMP/temp_${i}.txt"
# if frame is missing a scene, just leave it out
echo "frame number: $i until $END_FRAME"

for SCENE_NAME_PER_FRAME in `ls $WESTLING | grep ".*_$i.jpg" | cut -d '_' -f 1`
do
# loop for all frames of the final video and the second loop for all scene names, which already have rendered frames. scenename is read from the filename.

echo -n "$WESTLING/${SCENE_NAME_PER_FRAME}_${i}.jpg -geometry `SCENE_PIP_PER_FRAME` -composite " >> "$TEMP/temp_${i}.txt"
# the whole thing is put in a temp file for each frame; correctly formatted for the imagemagick command
# the -n tells echo not to use a new line parameter!!

done # end scene_name_pip_frame

convert -type TrueColor -size $OVERALL_ASPECT_RATIO xc:black `cat "$TEMP/temp_${i}.txt"` "$TEMP/output_`printf "%04d" $(( $i - $START_FRAME + 1 ))`.jpg"
# cat reads the temporary file and completes the command inside the loop. echo would just return the filename
# the usage of printf is necessary for ffmpeg in the next step
# type Truecolor explicitly needed, otherwise first black frame is saved in grayscale turning the whole video grayscale
# the term $(( $i - $START_FRAME + 1 )) is needed to always start counting from 0001 (the way ffmpeg requires it) even if the first frame is >1

done # end frames

echo "################ Render Video ######################"

DELAY_FROM_START_FRAME ()
{
printf "00:%02d:%02d.%03d\n" $(($START_FRAME/$OVERALL_FRAMERATE/60)) $(($START_FRAME%($OVERALL_FRAMERATE*60)/$OVERALL_FRAMERATE)) $(($START_FRAME%($OVERALL_FRAMERATE*60)%$OVERALL_FRAMERATE*1000/$OVERALL_FRAMERATE))
}
# brings the start_frame in the format mm:ss.xxx, this is needed for the audio
# 5/2=2 but 5%2=1, gives the remainder
# printf "%02d:%02d.%03d\n" $(($f/25/60)) $(($f%(25*60)/25)) $(($f%(25*60)%25*40))

# easy mpeg2 version
#ffmpeg -y -f image2 -i "$TEMP/output_%04d.jpg" -vframes $(($END_FRAME-$START_FRAME)) -r $OVERALL_FRAMERATE -b 10000k -ss `DELAY_FROM_START_FRAME` -i "shellac_mouthpiece.wav" -acodec copy "animation.avi"

# HD .mp4 version
ffmpeg -y -f image2 -i "$TEMP/output_%04d.jpg" -ss `DELAY_FROM_START_FRAME` -i "shellac_mouthpiece.wav" -vframes $(($END_FRAME-$START_FRAME)) -vcodec libx264 -vpre slow -crf 22 -r $OVERALL_FRAMERATE -threads 0 -acodec libfaac -ab 320k -ar 44100 -ac 2 "animation.mp4"

# -ss 00:00:002 start at (before the input file!) and -t 00:00:001 length
# -loop_input not needed

exit
```

## Appendix

ONE AFTER THE OTHER SCRIPT

It is the first I wrote, so please be careful. Corrections or optimizations are welcome. The programs used are: csvtool, imagemagick, ffmpeg.

```bash
#! /bin/bash

# variabels
BITRATE=600k
HEIGHT=x1080
# sets the absolute height
FRAMERATE_END=24
echo ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
echo "Please enter the SCENE's name or render all videos at once by typing all:"
echo ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
read INPUT_SCENE

if [ $INPUT_SCENE = "all" ]
################################################## BLOCK 01 #############################################################
   then
   echo +++++++++++++ "All scenes are processed" ++++++++++++
   echo +++++++++++++ "Reading parameters" ++++++++++++
   for ALL_SCENES in `csvtool drop 1 cutlist.csv | csvtool -t ';' col 2 -`;
   do
   RANK_ALL ()
   {
   grep "$ALL_SCENES" cutlist.csv | csvtool -t ';' col 1 -
   }
   FRAMERATE_ALL ()
   {
   grep "$ALL_SCENES" cutlist.csv | csvtool -t ';' col 3 -
   }
   LENGTH_ALL ()
   {
   grep "$ALL_SCENES" cutlist.csv | csvtool -t ';' col 4 -
   }
   echo "scene = $ALL_SCENES"
   echo "rank = `RANK_ALL`"
   echo "framerate = `FRAMERATE_ALL`"
   echo "length = `LENGTH_ALL`"
# warning about too many arguments, because finding lots of files?? but it works
   blod ()
   {
   find ./02_scenes/$ALL_SCENES -name `RANK_ALL`_${ALL_SCENES}*
   }
   if [ -z `blod` ]
# if the rank is not the same with the one in the cutlist it has to be updated
     then
     echo +++++++++++++ "Rename $ALL_SCENES by updating its name and rank" ++++++++++++
     for FILE in 02_scenes/$ALL_SCENES/*frame*.jpg ;
        do
        NEWFILE ()
        {
        echo $FILE | sed "s/${ALL_SCENES}\/.*_.*_frame/${ALL_SCENES}\/`RANK_ALL`\_${ALL_SCENES}\_frame/g"
        }
        mv "$FILE" `NEWFILE` ;
        done

#paths need to be preserved! wildcards with .* - no idea why!
#frame_* instead of more general *.jpgs because there are also the original photos in the directory
   fi

   echo +++++++++++++ "Render scene $ALL_SCENES" ++++++++++++
   ffmpeg -y -loop_input -f image2 -r `FRAMERATE_ALL` -i "02_scenes/$ALL_SCENES/`RANK_ALL`_${ALL_SCENES}_frame_%04d.jpg" -b $BITRATE -r $FRAMERATE_END -vframes `LENGTH_ALL` "03_output/`RANK_ALL`_${ALL_SCENES}_output.avi"
   done
#{} are necessary to preserve the following underscore
# -r framerate needs to be set before the input parameter
# the framerate of the output is necessary to keep the framerate differences of the scenes

   else
# if scene not in cutlist; ask for parameters, copy frames and write to cutlist
   if [ -z "`grep ";${INPUT_SCENE};" cutlist.csv`" ]
################################################## BLOCK 02 #############################################################
# semicolon prevents the matching of incomplete (parts of) scene names for instance "bdeckunge" instead of "abdeckungen"
# for condition (-z (string is null) -n (string is not null))
      then
      echo +++++++++++++ "${INPUT_SCENE} is not existing ... creation initialized" ++++++++++++

      echo +++++++++++++ "Have you cut the frames of ${INPUT_SCENE} to 4:3 aspect ratio?" ++++++++++++
      read -p "Of course I did!"

      echo +++++++++ "Define parameters" ++++++++++
      echo "Please enter its RANK (4 digits):"
      read INPUT_RANK
      echo "Please enter the framerate:"
      read INPUT_FRAMERATE
      echo "Please enter the length in number of frames:"
      read INPUT_LENGTH

      echo +++++++++ "Create directory for scene" ++++++++++
      mkdir -p 02_scenes/$INPUT_SCENE
# if directory is already existing, no error is given due to the -p

      echo +++++++++ "Copy frames to newly created directory" ++++++++++
# should be 4:3
      mv ~/*.jpg 02_scenes/$INPUT_SCENE

      echo +++++++++ "Resize frames" ++++++++++
      mogrify -resize $HEIGHT 02_scenes/$INPUT_SCENE/frame_*.jpg
# only frames, to prevent original photos;
# imagemagick is used for this

      echo +++++++++++++ "Rename by adding the scene's name and rank" ++++++++++++
# if the name is not congruent with the entries of the cutlist; rank is necessary for the order of the cat command later on
# only frames, to prevent original photos
      for FILE in 02_scenes/$INPUT_SCENE/frame_*.jpg ;
      do
      NEWFILE=`echo $FILE | sed "s/frame/$INPUT_RANK\_$INPUT_SCENE\_frame/g"` ;
      mv "$FILE" $NEWFILE ;
      done

      echo +++++++++++++ "Render $SCENE" ++++++++++++
      ffmpeg -loop_input -f image2 -r $INPUT_FRAMERATE -i "02_scenes/$INPUT_SCENE/${INPUT_RANK}_${INPUT_SCENE}_frame_%04d.jpg" -b $BITRATE -r $FRAMERATE_END -vframes $INPUT_LENGTH "03_output/${INPUT_RANK}_${INPUT_SCENE}_output.avi"
# {} are necessary to preserve the following underscore
# no overwrite (-y) needed
# the framerate of the output is necessary to keep the framerate differences of the scenes

      echo +++++++++++++ "Write variables to cutlist.csv" ++++++++++++
      echo "$INPUT_RANK;$INPUT_SCENE;$INPUT_FRAMERATE;$INPUT_LENGTH;" >> cutlist.csv
      read -p "Done!"
# as a last step after everything was successful to prevent errors in the cutlist

# if scene already in the cutlist
    else
################################################## BLOCK 03 #############################################################
    echo +++++++++++++ "$INPUT_SCENE is already existing" ++++++++++++
    echo +++++++++++++ "Read defined parameters of $INPUT_SCENE" ++++++++++++
# Define Functions RANK, FRAMERATE, LENGTH by reading cutlist.csv
    RANK ()
    {
    grep "$INPUT_SCENE" cutlist.csv | csvtool -t ';' col 1 -
    }
    FRAMERATE ()
    {
    grep "$INPUT_SCENE" cutlist.csv | csvtool -t ';' col 3 -
    }
    LENGTH ()
    {
    grep "$INPUT_SCENE" cutlist.csv | csvtool -t ';' col 4 -
    }
    echo "scene = $INPUT_SCENE"
    echo "rank = `RANK`"
    echo "framerate = `FRAMERATE`"
    echo "length = `LENGTH`"
    echo +++++++++++++ " The rank of $INPUT_SCENE changed ... renaming " ++++++++++++

# warning about too many arguments, because finding lots of files?? but it works
    blod ()
    {
    find ./02_scenes/$INPUT_SCENE -name `RANK`_${INPUT_SCENE}*
    }
    if [ -z `blod` ]
# if the rank is not matching the one of the cutlist, it needs to be changed
     then
     echo +++++++++++++ "Rename $INPUT_SCENE by updating its name and rank" ++++++++++++
     for FILE in 02_scenes/$INPUT_SCENE/*frame*.jpg ;
        do
        NEWFILE ()
        {
        echo $FILE | sed "s/${INPUT_SCENE}\/.*_.*_frame/${INPUT_SCENE}\/`RANK`\_${INPUT_SCENE}\_frame/g"
        }
        mv "$FILE" `NEWFILE` ;
        done
    fi
    echo +++++++++++++ "Render $SCENE" ++++++++++++
    ffmpeg -loop_input -f image2 -r `FRAMERATE` -i "02_scenes/$INPUT_SCENE/`RANK`_${INPUT_SCENE}_frame_%04d.jpg" -b $BITRATE -r $FRAMERATE_END -vframes `LENGTH` "03_output/`RANK`_${INPUT_SCENE}_output.avi"
# {} are necessary to preserve the following underscore
# the framerate of the output is necessary to keep the framerate differences of the scenes
    fi
fi

################################################## FINAL BLOCK #############################################################

echo +++++++++ "Remove expired output videos" ++++++++++
# remove expired output videos, otherwise cat adds them to the final file
for I in 03_output/*_output.avi
    do
    temp=`echo "$I" | cut -c 11- | cut -d '_' -f 1-2 | sed  "s/_/;/g"`
    if [ -z `grep $temp cutlist.csv` ]
        then
        echo delete $I ???
        rm -i $I
    fi
done
# the ls gives the path, cut removes the same path on the 11th digit and passes on the rest, cut separates the output at the '_' sign (recognizes fields) and provides the first two fields, sed is substitutes the '_' with a semicolon as used in the cutlist, and finally this string is looked up in the cutlist

echo +++++++++ "Merge all videos" ++++++++++
cat 03_output/*output.avi > 03_output/output_video.avi
# the rank must be correct for the sequence of the scenes

echo +++++++++++ "Add sound" +++++++++++
ffmpeg -y -shortest -i 03_output/output_video.avi -vcodec copy  -b $BITRATE -r $FRAMERATE_END -i 03_output/output_sound.mp3 -acodec copy "invent_a_fire.avi"
# should be a formality, the shortest input ends the the file
exit
```

# ! /bin/bash

# variabels

BITRATE=600k HEIGHT=x1080

# sets the absolute height

FRAMERATE_END=24 echo ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ echo "Please enter the SCENE's name or render all videos at once by typing all:" echo ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ read INPUT_SCENE

if [ $INPUT_SCENE = "all" ]

## ############################################ BLOCK 01

then echo +++++++++++++ "All scenes are processed" ++++++++++++ echo +++++++++++++ "Reading parameters" ++++++++++++ for ALL_SCENES in `csvtool drop 1 cutlist.csv | csvtool -t ';' col 2 -`; do RANK_ALL () { grep "$ALL_SCENES" cutlist.csv | csvtool -t ';' col 1 - } FRAMERATE_ALL () { grep "$ALL_SCENES" cutlist.csv | csvtool -t ';' col 3 - } LENGTH_ALL () { grep "$ALL_SCENES" cutlist.csv | csvtool -t ';' col 4 - } echo "scene = $ALL_SCENES" echo "rank = `RANK_ALL`" echo "framerate = `FRAMERATE_ALL`" echo "length = `LENGTH_ALL`"

# warning about too many arguments, because finding lots of files?? but it works

blod () { find ./02_scenes/$ALL_SCENES -name `RANK_ALL`_${ALL_SCENES}* } if [ -z `blod` ]

# if the rank is not the same with the one in the cutlist it has to be updated

```
 then
 echo +++++++++++++ "Rename $ALL_SCENES by updating its name and rank" ++++++++++++
 for FILE in 02_scenes/$ALL_SCENES/*frame*.jpg ;
    do
    NEWFILE ()
    {
    echo $FILE | sed "s/${ALL_SCENES}\/.*_.*_frame/${ALL_SCENES}\/`RANK_ALL`\_${ALL_SCENES}\_frame/g"
    }
    mv "$FILE" `NEWFILE` ;
    done
```

# paths need to be preserved! wildcards with .* - no idea why!

# frame __instead of more general_ .jpgs because there are also the original photos in the directory

fi

echo +++++++++++++ "Render scene $ALL_SCENES" ++++++++++++ ffmpeg -y -loop_input -f image2 -r `FRAMERATE_ALL` -i "02_scenes/$ALL_SCENES/`RANK_ALL`_${ALL_SCENES}_frame_%04d.jpg" -b $BITRATE -r $FRAMERATE_END -vframes `LENGTH_ALL` "03_output/`RANK_ALL`_${ALL_SCENES}_output.avi" done

# {} are necessary to preserve the following underscore

# -r framerate needs to be set before the input parameter

# the framerate of the output is necessary to keep the framerate differences of the scenes

else

# if scene not in cutlist; ask for parameters, copy frames and write to cutlist

if [ -z "`grep ";${INPUT_SCENE};" cutlist.csv`" ]

## ############################################ BLOCK 02

# semicolon prevents the matching of incomplete (parts of) scene names for instance "bdeckunge" instead of "abdeckungen"

# for condition (-z (string is null) -n (string is not null))

```
  then
  echo +++++++++++++ "${INPUT_SCENE} is not existing ... creation initialized" ++++++++++++

  echo +++++++++++++ "Have you cut the frames of ${INPUT_SCENE} to 4:3 aspect ratio?" ++++++++++++
  read -p "Of course I did!"

  echo +++++++++ "Define parameters" ++++++++++
  echo "Please enter its RANK (4 digits):"
  read INPUT_RANK
  echo "Please enter the framerate:"
  read INPUT_FRAMERATE
  echo "Please enter the length in number of frames:"
  read INPUT_LENGTH

  echo +++++++++ "Create directory for scene" ++++++++++
  mkdir -p 02_scenes/$INPUT_SCENE
```

# if directory is already existing, no error is given due to the -p

```
  echo +++++++++ "Copy frames to newly created directory" ++++++++++
```

# should be 4:3

```
  mv ~/*.jpg 02_scenes/$INPUT_SCENE

  echo +++++++++ "Resize frames" ++++++++++
  mogrify -resize $HEIGHT 02_scenes/$INPUT_SCENE/frame_*.jpg
```

# only frames, to prevent original photos;

# imagemagick is used for this

```
  echo +++++++++++++ "Rename by adding the scene's name and rank" ++++++++++++
```

# if the name is not congruent with the entries of the cutlist; rank is necessary for the order of the cat command later on

# only frames, to prevent original photos

```
  for FILE in 02_scenes/$INPUT_SCENE/frame_*.jpg ;
  do
  NEWFILE=`echo $FILE | sed "s/frame/$INPUT_RANK\_$INPUT_SCENE\_frame/g"` ;
  mv "$FILE" $NEWFILE ;
  done

  echo +++++++++++++ "Render $SCENE" ++++++++++++
  ffmpeg -loop_input -f image2 -r $INPUT_FRAMERATE -i "02_scenes/$INPUT_SCENE/${INPUT_RANK}_${INPUT_SCENE}_frame_%04d.jpg" -b $BITRATE -r $FRAMERATE_END -vframes $INPUT_LENGTH "03_output/${INPUT_RANK}_${INPUT_SCENE}_output.avi"
```

# {} are necessary to preserve the following underscore

# no overwrite (-y) needed

# the framerate of the output is necessary to keep the framerate differences of the scenes

```
  echo +++++++++++++ "Write variables to cutlist.csv" ++++++++++++
  echo "$INPUT_RANK;$INPUT_SCENE;$INPUT_FRAMERATE;$INPUT_LENGTH;" >> cutlist.csv
  read -p "Done!"
```

# as a last step after everything was successful to prevent errors in the cutlist

# if scene already in the cutlist

```
else
```

## ############################################ BLOCK 03

```
echo +++++++++++++ "$INPUT_SCENE is already existing" ++++++++++++
echo +++++++++++++ "Read defined parameters of $INPUT_SCENE" ++++++++++++
```

# Define Functions RANK, FRAMERATE, LENGTH by reading cutlist.csv

```
RANK ()
{
grep "$INPUT_SCENE" cutlist.csv | csvtool -t ';' col 1 -
}
FRAMERATE ()
{
grep "$INPUT_SCENE" cutlist.csv | csvtool -t ';' col 3 -
}
LENGTH ()
{
grep "$INPUT_SCENE" cutlist.csv | csvtool -t ';' col 4 -
}
echo "scene = $INPUT_SCENE"
echo "rank = `RANK`"
echo "framerate = `FRAMERATE`"
echo "length = `LENGTH`"
echo +++++++++++++ " The rank of $INPUT_SCENE changed ... renaming " ++++++++++++
```

# warning about too many arguments, because finding lots of files?? but it works

```
blod ()
{
find ./02_scenes/$INPUT_SCENE -name `RANK`_${INPUT_SCENE}*
}
if [ -z `blod` ]
```

# if the rank is not matching the one of the cutlist, it needs to be changed

```
 then
 echo +++++++++++++ "Rename $INPUT_SCENE by updating its name and rank" ++++++++++++
 for FILE in 02_scenes/$INPUT_SCENE/*frame*.jpg ;
    do
    NEWFILE ()
    {
    echo $FILE | sed "s/${INPUT_SCENE}\/.*_.*_frame/${INPUT_SCENE}\/`RANK`\_${INPUT_SCENE}\_frame/g"
    }
    mv "$FILE" `NEWFILE` ;
    done
fi
echo +++++++++++++ "Render $SCENE" ++++++++++++
ffmpeg -loop_input -f image2 -r `FRAMERATE` -i "02_scenes/$INPUT_SCENE/`RANK`_${INPUT_SCENE}_frame_%04d.jpg" -b $BITRATE -r $FRAMERATE_END -vframes `LENGTH` "03_output/`RANK`_${INPUT_SCENE}_output.avi"
```

# {} are necessary to preserve the following underscore

# the framerate of the output is necessary to keep the framerate differences of the scenes

```
fi
```

fi

## ############################################ FINAL BLOCK

echo +++++++++ "Remove expired output videos" ++++++++++

# remove expired output videos, otherwise cat adds them to the final file

for I in 03_output/*_output.avi do temp=`echo "$I" | cut -c 11- | cut -d '_' -f 1-2 | sed "s/_/;/g"`if [ -z`grep $temp cutlist.csv` ] then echo delete $I ??? rm -i $I fi done

# the ls gives the path, cut removes the same path on the 11th digit and passes on the rest, cut separates the output at the '_' sign (recognizes fields) and provides the first two fields, sed is substitutes the '_' with a semicolon as used in the cutlist, and finally this string is looked up in the cutlist

echo +++++++++ "Merge all videos" ++++++++++ cat 03_output/*output.avi > 03_output/output_video.avi

# the rank must be correct for the sequence of the scenes

echo +++++++++++ "Add sound" +++++++++++ ffmpeg -y -shortest -i 03_output/output_video.avi -vcodec copy -b $BITRATE -r $FRAMERATE_END -i 03_output/output_sound.mp3 -acodec copy "invent_a_fire.avi"

# should be a formality, the shortest input ends the the file

exit
