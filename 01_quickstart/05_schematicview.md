# Fritzing helping section #

# Everything about the software #

## Make your first steps ##

### Welcomeview ###
![](images/01_welcomeview.png)

1. Information and Updates
	
	The welcomeview offers a window into the makerworld. we provide you with updates from the blog and the community.
 
2. Projectgallery
	
	The project-section show you the latest updates from the community. You can find inspiration and allready made openHardware projets from other fritzing users.
  
3. recent file handeling
	
	The Recent-file frame shows a list of your last projects. so you can easily rejoin your last work.

4. Tips & Tricks

	This section provides you randomly with usefull tips and tricks for a better handling of fritzing.

### Breadboardview ###

#### 1. Building a Circuit ####
 	
1. Starting a new project:

	Before starting a project in Fritzing, you will need to build an electronic circuit in the real world and make sure it works properly. You will then virtually rebuilt the circuit in Fritzing.
	Let's start by opening Fritzing, naming and saving our project. Saving a project is highly recommended at start and every now and then while working, since Fritzing is still Alpha and unfortunately might sometimes crash...

	1. From the Fritzing menu bar select File > Save As...<p>
	![](images/02_save-as.png)

	2. Specify a name and location for the project and click Save<p>

	
2. Arranging the environement

	Before we start working, we might want to arrange the environment according to our needs and preferences.
	1. From the Fritzing Menu Bar, select Window > and mark the palette windows you would like to see in the environment.<p><p>
	![](images/03_palettearrange.png)
	2. Drag & drop palette windows anywhere in the environment and notice how windows rearrange, combine or float.
	3. Choose the breadboard view in the Navigator, in case it is not already selected.<p><p>
	![](images/04_breadboardview.png)

3. Building a circuit

	Make sure your circuit in the real world works properly. Then rebuild your circuit in Fritzing following these guidelines:
	1. Drag & drop an Arduino or another Microcontroller of your choise from the Parts palette window to the Project View.<p><p>
	![](images/05_droparduino.png)
	2. Do the same with a breadboard and all other parts of your circuit. If you cannot find a part in the library, use the Mystery Part (icon looks like a qustion mark - ?). The Mystery Part will let you quickly define a new part and its connectors (through the Inspector). Or use the generic ic. it has e.g. multiple smd footprints. 
	3. You can arrange parts by selecting, dragging and dropping, or by using the functions in the menu bar, located under Part.
	4. To delete a part, simply select and press BACKSPACE or Del.
	5. Click & drag the Arduino +5V connector. This should create a wire. Drop the wire on one of the breadboard's connectors. The connection is confirmed by a small green circle or square.
	6. Connect all parts until the circuit looks exactly like your circuit in the real world. Notice that connectors that are not properly connected are painted red.
	7. If you click and hold on a connector, Fritzing will highlight all equipotential connectors. This can really be useful if you want to see the whole set of connections attached to this particular connection.
	8. You can bend wires by adding bend-points. Just drag them out of a wire. Hit strg on a wire to make it curved.<p><p>
	![](images/06_firstcircuit.png)
	9. Select the schematic and pcb tabs to watch or edit your circuit in these views. <p>

1. Editing properties

	Now that we have all parts connected, let's see how we can modify the properties of each part.
	1. Select any of your circuit's parts and have a look at the Part Inspector palette window.
	2. Click on the part's name and rename it. This is useful when you want to distinguish between similar parts.
	3. Try also to change other properties.<p><p>
	![](images/07_properties.png)
	<p>
	You can also change properties of parts in the PCB View. The board's shape could be changed to an Arduino shield, a resizable rectangle or a custom shape.	


1. Exporting a circuit

	After finishing building the circuit, save your project. You might want to export your circuit as an image file or PDF.
	1. Select the desired Project View to be exported (breadboard,schematic or pcb).
	2. From the Fritzing menu bar, select File > Export > and the desired format.<p><p>
		![](images/08_export.png)

#### 2. external learning material ####

1. Using a Stripboard (from the video channel)
2. Working with SMD parts (from the video channel)
3. Creating Paper Templates (from the Blog)
4. Curvy Wires and bendable Legs (from the Blog)

### Schematic View ###

#### 1. how to use ####

The schematic view is the classical way to communicate about builded circuits. It's aim is to document your
circuit in a way an electrical ingeneur works with electronics.

1. the componets you used in the breadboardview are now symbols. the electrical connections you build in breadboardview are now visible in these dotted lines. let's call them "ratsnest".<p><p>
	![](images/09_sortparts.png)

2. sort the componets around the arduino board. <p><p>

3. make wires from the ratsnest<p><p>
	![](images/10_ratsnest.png)

4. look at the clean schematic diagram you have now from your circuite.<p><p> 
	![](images/11_wiredschematic.png)

If you now ask yourself of the need of this view it's somekind of normal. But if you use it more and more, you will discover how easy it is to read schematic from allready developed things and you could even start from a schematic to build a prototyp or test circuite. 	


### PCB view ###

#### 0. Before we start ####
Fritzing's PCB View lets you design and export layout files for single-sided, DIY Printed Circuit Boards. You can also export your sketch to Gerber files, and send them to a professional PCB manufacturing service or easily use the [Fritzing-Fab-Service](http://fab.fritzing.org). The Service makes it possible for you, ordering your designed board, directly from the fritzing fzz file, as a professional pcb. Once you get to know Fritzing's PCB design tools and functions, creating a nice layout will become easier.
Changes in the software are constantly being made in order to improve and make this process easier for you, so please be aware that some bugs might come and go... 

To learn how to use Fritzing's PCB design tools, go through the following steps and guidelines.

#### 1. the PCB view ####
So your circuit works and also looks great in Fritzing's Breadboard View.<p><p>

![](images/12_breadboard-pcb.png)<p>

Let's now have a look at the PCB View. To switch to the PCB View use the Navigator or the View Switcher. While it is very easy to recognize parts in the Breadboard View, the PCB View might look a bit confusing at first glance. The reason for this is that the PCB View only shows the necessary information needed for the PCB design. This information is shown in different layers. To view or hide layers, use the View options in the menu bar. Learn more about the PCB View layers.
As an example, lets have a look first at the following circuit which was created in Breadboard View:<p>
 
![](images/13_pcbview.png)


Selecting PCB View in the Navigator will show a completely different illustration of the same circuit. 
The with rectangle is the board itself, on which parts will be arranged. It is automatically placed as you open a new sketch. 
Parts are shown as footprints, including the Arduino footprint, and you can identify them by selecting or placing the cursor on them to see their labels. 
The thin connecting lines are the Rat's Nest (more about the Rat's Nest below).
 
You might want to resize the board, or use an Arduino shield or a board with a custom shape. Select the board and choose/edit your prefered shape in the Inspector.<p><p>

![](images/14_changepcbshape.png)


#### 2. Arranging parts on the board ####
The first step in designing a PCB layout is arranging the parts on the board. 
There are some very important issues to consider here, because the location of parts on the board will have a great effect on how successful the routing process will be.
Follow these guidelines:

1. Place the parts with the most connections in the middle of the board. 
2. Notice that Arduino's footprint should also be positioned on the board, just like other parts.
3. Rotate and position parts, leaving enough space between them (don't forget their actual size!).
4. Use a grid like 0.1inch or 0.05inch. Most of the parts fits into this grid and it makes the design process much easier and faster. 
4. If the board is too small, redefine its width and height in the Inspector or alternatively resize the board by dragging its corners. **Learn how to design a PCB with a custom shape.**
5. Don't place parts too close to the edges of the board.
6. To avoid short circuits, don't place parts too close to the USB connector outline on the Arduino Shield.
7. When designing stack shields, parts' heights should also be considered.

The following screenshot shows one out of many possible part arrangements for the given circuit:<p><p>
![](images/15_pcbarranged.png)

#### 3. Hand-routing ####

Use any of the following methods to hand-route traces and jumpers:

1. The safest way is to right-click a Rat's nest wire and choose "Create Trace from Selected Wire(s)" or "Create Jumper from Selected Wire(s)". This will avoid making any changes in the circuit that you built in Breadboard View.<p><p>
![](images/18_ratsnesttotrace.png)

2. Another way is to simply click a part's connector, and drag to make a connection. A trace will be created. To create a jumper, just right-click on the trace and choose "Create Jumper from Selected Wire(s)". To avoid incorrect wiring, we strongly recommend you follow the Rat's nest wire connections while using this method.<p><p>
![](images/20_dragratsnest.png)
3. You can use both sides of the pcb to make a suiteable wireing. So it is possible to sent traces to top and bottom of the pcb.
<p><p>
![](images/21_topbottom-trace.png)

Note that while clicking and holding on a connector, all equipotential connectors are highlighted (in yellow). This shows the whole set of connections attached to this particular connection, and can really help to make hand-routing decisions. Once again, take good care not to cross wires!<p><p>
![](images/22_highlightedconnections.png)
#### 4. Auto-routing (not recommanced) ####

After positioning all parts on the board, be aware that parts are not really connected to each other yet. The thin connecting lines that you see (Rat's Nest Layer) only act as a guideline. We would now want Fritzing to automatically generate the connection traces between parts. Click the Auto-route function from the bottom menu bar. 

If you notice that Fritzing is struggling trying to generate a connection, you can press the "Skip this Trace" button or "Cancel Auto-routing" in the bottom menu while in process.<p><p>
![](images/16_autorouter-process.png)

Such a problem might happen because parts were not arranged properly on the board or when there is just no possible route. You will then need to Hand-route the trace or create a jumper. Jumpers are connections that need to be soldered with external wires. These are shown as blue connections while traces are shown as orange ones.<p><p>
![](images/17_autorouted.png)

If you are happy with some of the traces and want to keep them untouched, or you know in advance that some connections need jumpers, you might want to tell Fritzing to exclude some connections in the auto-routing process. To do so, select the connections you want to exclude, choose "Don't Autoroute this trace" in the right-click menu or in the Trace menu. Only then press Auto-route. The selected traces will be left untouched while all other connections will be auto-routed. Any traces that were handrouted are automatically marked as "Don't Autoroute."<p><p>
![](images/18a_dontautoroot.png)

Be aware that if you moved a part after auto-routing or hand-routing, the routing traces are not corrected automatically. You will need to be cautious when moving parts and make sure you don't create any short circuits.



#### 5. Guidelines for better routing ####

For both auto- and hand-routing, follow these guidelines:

1. Place the parts with the most connections in the middle of the board.
2. Try to get short connections by moving and rotating parts.
3. Use the highlighting of equipotential connectors feature.
4. Add bend points for tidy routing and so that lines do not cross.
5. Don't forget the traces can go under parts like resistors.
6. Use jumper wires instead of watching the auto-route go crazy.
7. Choose a good grid (e.g. 0.1inch) and "align to grid"-option for a straight forward routing and design process<p><p>
![](images/23_setgrid.png)

#### 6. Editing Traces ####

To achieve a better and nicer design, you would need to edit traces by moving, adjusting width and adding bend points. Width adjustment can be done in the Inspector. Please note that thin traces might ruin in a DIY PCB production, so keeping traces in medium thickness is safer. To create a bend points drag it simply out of a trace.<p><p>

![](images/24_add-bentpoint.png)

Sometimes, it would be possible to edit traces in a way that will reduce the number of  jumpers. The routing in the screenshot above was edited and a better design was achieved:<p><p>
![](images/25_goodroute.png)

#### 7. Export Options ####

Fritzing features a variety of export options. When you are happy with your PCB design, you can choose to export JPG, PNG, etchable PDF and even Gerber files (for sending a professional PCB manufacturing service). The Bill of Materials option generates a list of all parts in the circuit.
From the menu bar choose File > Export > and the desired format.

- For DIY PCB production, use the Etchable PDF option which exports only the necessary design for etching.
- When exporting Gerber files, create a folder for the gerbers, and zip. it before sending to a manufacturer.<p><p>
![](images/26_export-diy.png)

Or you try the [Fritzing-Fab-Service](http://fab.fritzing.org) by useing the "Farbricate" button in the pcb-views bottom. it will let you order directly from the fritzing sketch. Hovering the button gives you a feeling about the fab-price per board and the discount if you need more copies.<p><p>	
![](images/27_fabricated.png)

So hopefully, this tutorial helped you understand the PCB design process. Good luck and show us what you've done!<p><p>


# everything about parts #

## Creating custom Parts ##

Many projects require the use of some very specific parts and as we cannot provide them all, we try to make it as easy as possible for you to create your own.
Be sure to check Fritzing's library before you start creating a new part. Often there would be a quicker way to get what you need, like using a generic part or by modifying an existing part. Follow one of the two ways:

### 1. Using generic parts ###
Standard parts like ICs, resistors, and pin headers can be defined easily by using Fritzing's generic parts. <p><p>

![](images/28_generics.png)

For example, the name and number of pins of the IC part can be defined in the pulldown menu inside the Inspector:
<p><p>

![](images/29_generic-ic-pins.png)<p><p>
and the result is...<p><p>
![](images/30_generic-ic-result.png)
 
It might be important for you to define some more part specifications (properties, connector names, etc.) and you would probably also want to save your part. To do so, select your part and edit it using the Part Editor (Part > Edit(new parts editor)). For more information, please check the following pages:

#### 1. First steps in the Partseditor ####

Fritzing-parts working on xml and svg basis. It is not possible to use rasterd images like e.g. jpg or png. A part needs at least 4 files. 3 svg-graphics for the part and an xml-file, the fzp. A part-file (fzpz) is a normal zip-archive. Anyway, the fzp defines the part, which means all the properties and connectors and the svg-files for the specific views. 
It is possbile to modify the parts fzp in the Metadata- and the Connectors-Tab (more information will follow below). It is planed to be able to modify the parts-svg itself in the editor. But for now it is not yet possbile. 
We recommance the use of the free openSource vector-programm [InkScape](http://www.inkscape.org/). Other comercial programms are e.g. Adobe Illustrator and CorelDraw (or if you are a pro use a simple editor to modify the svg.)

**The Partseditor**<p><p>

1. First of all, the parts editor do not let you begin from scratch, so you need to find a part that is close to the one you want to create. That means:

	How many connectors you need?
	What kind of housing you need? (smd or tht)	

2. Drop the chosen part in the sketch window, make a right-click and choose "Edit (new parts editor)"<p><p>
![](images/31_edit-partseditor.png)

3. Now the Partseditor-window came up. It has six tabs. The first four viewes let you define the graphic of the part and the icon that gets used in the library. 

4. We start now in the breadboard-view of the part. On the right you see all the defined connectors.
***NOTE** if you have a part with many connectors it can safe you a bunch of time beginning with the connectors-tab because all the connectors listed here and can be simply modified*<p><p>
![](images/32_editor-bread.png)

5. You can find the svg for this view simply by "File > show in folder". It is strongly recommanced to copy the svg to another place before editing it. Otherwise you will destroy the fritzing-core-part.

6. Now open the copied svg and make the changes you need for the part. ***NOTE** at this point you need to know how a vector-programm is used to make the modifications. Have a look in the external link section for good tutorials concerning this topic.*   

7. Now you want to use the self created or modified svg for the view. Therefor use the menu and select "load image for view". Navigate to the location of your svg and load it. Now the Partseditor shows the new image.<p><p>
![](images/34_editor-loadforview.png)

8. By hovering over the loaded parts-svg you will see a blue highlighting. If you click on "Select graphic" for one of the connector-pins the highlighting becomes mangenta. Now you can choose one of the part-svg-paths that will be used for the connector. By holding shift + useing the mousewheel you can easily access all the paths form the svg overlapping each other. By using the left mouse-button the chosen path becomes the new connector. <p><p>
![](images/33_editor-select-connector.png)

9. The other two views, Schematic and PCB, acting nearly the same way. 

10. The Icon-tab provides the symbol that the part will use in a fritzing-library.

At this point there are two really important tabs left.  

#### 2. Metadata-Tab - Defining Part Specifications ####

Here you can change all the properties for the part. That includes e.g.:

- **Title** - it is sometimes useful to choose a name which is descriptive, specifying for example color and size.
- **Label** - helps keep track of the parts in your circuit, by numbering your parts based on this label. For example, LED1, LED2. When you are ready to manufacture a PCB, this will be extremely helpful in figuring out which part gets soldered where.
- **Description** - A brief description about your part that gives a few useful details, tips or links.
- **Properties** - the part's technical characteristics. Enter all of the distinguishing features that make your part unique. First enter the family your part belongs to such as, LED, photo resister, etc.
- **Tags** - makes your part findable. Enter words into the Tags field that will make your part show up in a search. Family should always be one of these tags.
- **URL** - enter a link to the datasheet of the component for reference and more information
- **Author; Created/Updated on** - Let your friends know how cool you are, enter your name! While you're at it, let them know when you were that cool.
 
When you are done defining the part specifications, go through it once again to make sure all necessary information has been inserted.
In the next step, we will define our part's connectors.

#### 3. Defining Part Connectors ####

In the connectors tab you can specify the individual connectors of your part. This is done in three steps:

1. **Add or modify a connector pin** - the connector pin represents the active connection area, that is the area where wires can attach to your part. To define the number of connectors, simply type the number into the field and hit enter. Now the connectorlist shows as many connectors you have defined.  Its time to go to every connector in the list and fill out the Name and Description fields (according to the part's data sheet, for example Name: VDD ; Description: Positive Supply Voltage). You can change the type of the connector between male, female and pad (the connectortyp for smd parts) by clicking the icon on top of the list or on the right of the name field. It is important to check that the housing type of the part is set the right way. The question is do you make an SMD or an Through-hole (THT) part?

[image]

2. Position and resize the connector pin - this must be done in each of the three graphics. Just drag the connector pin and place it at the proper location (for example on the part's leg). You can also resize a connector accordingly by pulling its corners. The zoom function allows you to place and position your pin connectors much more accurately, so keep it in mind!
3. Position the anchor point (optional) - Anchor points represent the point of connection and influence how wires and traces extend from your part. In the Breadboard View the terminal point will be the end of your pin, where the wire will connect. In the PCB View the terminal point will define traces and holes in the physical PCB. Check the Show Anchor Points box, and drag the little '+' sign in each view to the proper location. If you do not position the anchor point, it will be automatically positioned at the center of the connector pin.
 
[image]

When you're done, click save as new part.
That was it... your new part is now saved in the "Mine" bin. Before you start using it, go on to the next step to test and make a quality check for your part.

[image]

#### 4. Testing & Quality Check ####

Once you've created your part, you may want to give it a quality check by going through this list of questions.

**Part Graphics:**

- Does the part look like the component it's supposed to represent in all three views?
- Does the part contrast enough on the breadboard?

**Part Properties:**

- Do all part properties show up in the Inspector correctly?
- Can you change the part's properties in the Inspector? (when the part belongs to a certain family)

**Part Connectors:**

- Does the part fit in the breadboard?
- Do connectors turn green when components are placed in the breadboard?
- Can connectors be individually selected and wired, in all three views?
- Is the selection area on the part in the correct place?
- Do colors of connectors contrast enough to be seen and be selected?
- Based on a datasheet, are the connectors labeled correctly and consistently in all three views?

#### 4. Using & Sharing ####
Now that your new part is ready, you can share it with friends and with the Fritzing community.

**Exporting a part**

To export your part, select the part in the Part Library and click the part icon at the bottom of the library. 
Choose "Export...", then specify a name and location to export.
Your friends can import your part to their own Fritzing library by selecting "Import..." from the same part menu.

 
**Finding a part on your system**

Sometimes, you might want to access and re-edit a custom part's graphic. To do that, click the "image..." link under the graphic, choose the relevant .svg file and drag (mac: +alt) to copy it to a different location. Then open the file with Illustrator/inkscape and edit it (creating your graphics in SVG format). When you're done, click the "image..." link again to import the edited graphic and click "save as new part".
Please note that Fritzing keeps your custom parts and bins in your user folder on your system, so that when you upgrade to the next Fritzing version, all are instantly accessible. Under Windows Vista/7, that's C:\Users\<username>\AppData\Roaming\Fritzing, under Win XP it's C:\Documents and Settings\<username>\Application Data\Fritzing, and under Mac OS X it is /Users/<username>/.config/Fritzing. These folders might be hidden by default.

If you still encounter problems finding your custom parts in a new upgraded version, try to import them manually by selecting Help>Import parts and bins from old version... . Navigate and locate your old Fritzing folder and press "choose".

### 2. Creating custom parts using the Part Editor ###


#### 1. part-creation - first step ####
When your project involves a part that does not exist in Fritzing's core part library, and the part cannot be created using a generic part, you will need to use Fritzing's built-in Part Editor.
Before using the Part Editor, you should think whether it makes sense to build your part from scratch, or maybe there is already some part in the library which has similar graphics that could be modified. You could then change whatever needed and save the part as a new one. This will surely save a lot of time.
 
To modify an existing part, select a part in the Project View and then Part > Edit .
To create a part from scratch, open the Part Editor under Part > New in the menu bar.
 

 
At the top of the Part Editor you will find the name field. Lets start by naming our new part.
 

 
Further down is the part's graphic fields as well as the part's properties which are arranged in two main categories: Specifications and Connectors.
 
In the next step, we will go through the process of providing part graphics.

#### 2. Providing Part Graphics ####

Every Fritzing Part must have 3 different graphics for each of the 3 different views (Breadboard, Schematic and PCB), plus an icon for the parts bin. SVG, PNG and JPEG formats are supported (except for the part's pcb graphic which must be an SVG for the gerber files export to work well).

Using JPEG & PNG images is the easiest and fastest way to get things done, although zooming might pixelate your image. If you are interested in sharing your custom parts with the Fritzing community, we strongly recommend using a vector graphic editor to draw all part's graphics in SVG format.

You can use the open-source tool Inkscape (free and cross-platform), the commercial tool Adobe Illustrator (costly and Win/Mac only), or any other vector drawing tool that supports the SVG Tiny or Basic standards (see this list of tools).

Before you start creating your own graphics, check the existing graphics in the subfolders at Fritzing>parts>svg>core and Fritzing>parts>svg>contrib. Especially when you need to create a custom PCB footprint, the contrib folder can save you a lot of work.

Let's start with the breadboard and schematic graphics. Use the template files or modify an existing part's graphics following these rules:

1. Design according to Fritzing's graphic standards.
2. When modifying an existing part, never rename its connector paths.
3. Do not use any effects such as gradients and other bitmap effects.
4. Use the part's datasheet and use a caliper so that you can get the correct external dimensions and reliable information about the part's specifications. You will also find the schematic symbol in the datasheet, which you can use for the schematic view graphic.
5. A graphic for the PCB View should be grouped according to the different PCB layers. Open an existing footprint in Inkscape to understand how it is done.

[image]

Now make your SVG compatible with Fritzing:

1. Delete all graphical artefacts like masks, meshes and styles.
2. Delete all unnecessary layers (for example a breadboard image that you used as reference).
3. Rearrange all graphical elements inside a single layer.
4. Group all graphical elements and rename this group according to what it represents (“breadboard”, "schematic", "pcb" or "icon").
5. Resize the art board to the external dimensions of the part:
Inkscape: select the group, then go to "File>Document Properties" and click on "Fit Page to Selection". 
Illustrator: use the crop tool and option “Fit crop area to Artwork bounds". 
Please Note: a bug in illustrator might cause the graphics to move from the crop area after saving. Close and open the file again, use the grid and drag (do not align!) the graphics to the upper left corner of the crop area, making sure all graphics are within. Save the file again, close and open it to check that the graphics are now placed correctly.
6. Save it in SVG format (without any program-specific add-ons):
Inkscape: Save your file as a "Plain SVG" (not as Inkscape SVG)!
Illustrator: Save your file as SVG with the SVG profile Tiny 1.2 or Basic 1.1.
CorelDraw: Export your file as SVG and in the styling options choose "presentation attributes" (also see forum).

[image]

Once you're done, import the new breadboard and schematic graphics to the Part Editor by clicking the "image ..." link under each of the corresponding graphic fields. To import a new pcb graphic, navigate to the footprint svg. files at Fritzing>parts>svg>core>pcb. Find the footprint that fits your new part and click "open". In case you cannot find the correct footprint for your part, try modifing an existing footprint.

[image]

The parts bin icon represents your part in the Part Library. It can be created from a minimized version of the breadboard view graphic. This should be a 32x32px image and can be imported to Fritzing by clicking the "image ..." link under the small icon field at the upper left corner of the Parts Editor.
 
In the next step, we will define our part's specifications.
-> see 1. Defining Part Specifications

### 3. make a custom pcb-shape ###

Fritzing lets you design your PCB in any size and any shape. When you start working on a new sketch, a default rectangular board is placed in the PCB View. You can then define width and height in the Inspector or alternatively resize the board by dragging its corners. You can use the shape popup in the Inspector to switch to an Arduino shield shape or an ellipse.

To use boards with more complex shapes, create your board's shape with an external SVG editor (Inkscape, Illustrator, etc.) and then import it to Fritzing. Follow these steps:

1. Design an SVG with two sub-groups:
	- A "board" group with a path in any shape and size. The shape should be filled white and should not have any stroke. 
	Make sure you only have a single merged shape, not serveral distinct ones. If you want to display some guiding graphics (such as the location of the pin headers for the Arduino shield), you can add them as sublayers of "board". In this case, make sure you give the board shape item itself the id "boardoutline". That is to say, although we talk about "layer" the SVG attribute you actually set is "id".
	- A "silkscreen" group with a copy of the path you've just done, this time with no fill and with white stroke (for Inkscape users: stroke = 8 mil). Make sure the silkscreen layer is arranged at the top. Remember to set the "id" attribute to "silkscreen", not the "group" attribute.
 
    >      <svg>
    >      [...]
    >      <g id="silkscreen"></g> 
    >      <g id="board"><path id="boardoutline"/></g>    
    >      [...]
    >      </svg>

2. Illustrator Users: Align all elements to the center of the artwork
3. Illustrator Users: Use the crop tool and choose the preset "fit crop area to selected art"
	
	[image]

4. Save the file as an SVG Tiny 1.2.
	[image]

6. Drag a plain PCB to the PCB View.
7. In the Inspector, select "import shape" from the shape drop down menu, navigate to the SVG file and press "Open". Your custom PCB shape is ready to use!
You can inspect this sample shape to get a further sense of the details. Note again the use of the "id" attribute. 

**Illustrator Users**, please note. If you use Illustrator to make your custom board svg, and you notice that the board size is not correct in Fritzing, this is because Illustrator uses non-SVG-standard units for pixels.  In Illustrator-world, there are 72 pixels per inch, but the rest of the svg universe uses 90 per inch. Fritzing usually catches this, but if it doesn't, try the following: open up the svg in an text or xml editor and find the width and height attributes in the top level (<svg>) element, which will have units of "px".  Divide the value of the width and height attributes by 72, and replace the current attributes with that new number followed by "in".  For example, if you see width="100px" replace it with width="1.3889in".  

**Inscape users**, please note. When we say set the "id" to 'silkscreen' or 'board' or 'boardoutline' we do not mean the 'label' attribute. The 'id' is the very first text input area in the Object Properties dialog--the label is the second. You can also set this using the XML editor under Inkscape's Edit menu.

**Inscape users**, please note. We also strongly recommend that you save Inkscape files as "plain SVG" before you import them into Fritzing. You can choose this option by selecting 'Save As' and in the dialog that comes up, choose 'Plain SVG' from the "Save As Type" popup near the bottom of the dialog.

# be an advanced fritzinger #

# FAQ #
1. ratsnest? what is it good for?
2. copperblocker? how it works
3. what can i do if my specific part isn't avalible
4. should i update my fritzing to the newst version?
5. 