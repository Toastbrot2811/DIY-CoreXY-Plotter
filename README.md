In my electrical engineering Class, I was tasked to Create a Presentation about the Stepper motor and to create a little project with it and an Arduino or a similar micro controller. The expectation was to have something like a clock, or some other simple project, to show off the basic functionality of a stepper motor. I wasn't really satisfied with these simple projects, so I asked Chat GPT for some project ideas for my presentation and it proposed the idea to build a pen plotter. Plotters were alway fascenating to me and due to my decent knowledge of 3D-printers and the Marlin 3D-printer firmware I was confident, that I would be able to build my own plotter from scratch in about 3-4 weeks. My goal was, to build it as cheap as possible, because I'm a poor student and didn't want to spend more than 100€ on a school project. This meant, that I was constrained to parts, that I could get from an old 3D-printer, which start at around 20€ here in Germany. So I started to do some research and found an old Anet A6 3D-printer on an online marketplace (Kleinanzeigen) for just 25€, which was complete and had a motion system built from linear rods and bearings, which was perfect for my project. 

![20250214_201416](https://github.com/user-attachments/assets/1b3c48e2-0601-42b7-9994-4e1d8622f569) 

The printer was of course rather janky and was falling apart everwhere, but all the parts I nedded, which are like all of them accept the frame and the heated bed, were there and in workable condition. So one hour and what felt like 5 million M3X18 screws later I converted the 3D-Printer into a pile of parts.

![20250214_213416V2](https://github.com/user-attachments/assets/f645dc16-342c-4bcf-bbf5-c78fabb4b242)

Then it was on to designing the whole thing in fusin360, which took around 20 hours wih my limited CAD experience. 

I startet with the toolhead, because it was the most complex part of the whole plotter. I designed it to be modular and to have a low center of gravity, while only using parts from the Anet A6. This is why the stepper motor is on below the linear rods. The setup with a complete Z-axis is of course overkill for a simple pen plotter, but it makes it simple to programm and it allows you to use the stock mainboard without any modifications. It also gives you the option to reuse most of the parts if you want to convert the plotter to a laser cutter (coming soon). 

![20250225_224527](https://github.com/user-attachments/assets/8865cc1e-5efa-49d2-b977-23cdf8537563)

So after alot of measuring and 3D-modeling, I had the first prototype of the Z-axis. 

For recreation:

Use one of the shortest 8mm linear rods from the printer and cut a 146mm long piece from it with an angle grinder or a dremel, because of the hardened steel. For the threaded rod, you can use a regular saw, to cut off a ~87mm long piece. make sure to clean the threads on the cut. 
To 3D-print the plastic parts, use PETG or ABS/ASA and at least a 0.6mm nozzle with a 0.35mm layer hight. For my build, I used the before mentioned printer settings on PETG-CF for the extra stiffness, but you don't have to. All M3-screws, that srew into the plastic use M3X4 heat set inserts in this project.

How to build the Z-axis:

1. Print out all the Parts of the Z-axis
2. Take the linear beraings from the original print head and press them into the base of the Z-axis. You can use the original grub screws if you want to fasten the bearings, but that was not necisary in my case.
3. Take the origninal X-axis limit swich and screw it into the Z-axis base with the original screws. The rear screw is currently very hard to reach, I may add an extra access hole in the future.
4. Assemble the stepper motor and the short treaded rod, whith the included coupler and bolt the stepper motor with the threaded rod into the base with 4 M3X12 bolts.
5. Use a soldering iron to melt M3X4 heat set inserts into all holes on the base, which have a 4mm diameter.
6. Bolt the front support pillars into place with atleast 4 coutersunk M3X10 screws.
7. Take the pencil holder and bolt two of the bearing blocks from the old print bed to it, with the inclued M4 bolts. Then use the heat set inserts and screw the pencil clamp onto the pencil holder with two M3X20 bolts.
8. 
