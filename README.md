Various ULPs (User Language Programs) for the Cadsoft EAGLE
=============

align_objects.ulp
=============
An ULP to align the selected objects centered on straight line either horizontally or vertically.

Add the following sections to the .eaglerc (or whatever it is on Windows), and copy the resources/align_objects/action_icons folder to the bin folder of your EAGLE installation and you will be able to use it from the context menu:

*Sch.MenuText.01 = "[align.png] Align selected objects { [format-justify-top.png] Align to top: Run align_objects.ulp vtop; | [format-justify-bot.png] Align to bottom: Run align_objects.ulp vbot; | [format-justify-left.png] Align left: Run align_objects.ulp hleft; | [format-justify-right.png] Align right : Run align_objects.ulp hright;}"*

*Brd.MenuText.01 = "[align.png] Align selected objects { [format-justify-top.png] Align to top: Run align_objects.ulp vtop; | [format-justify-center_v.png] Align center vertically: Run align_objects.ulp vcenter; | [format-justify-bot.png] Align to bottom: Run align_objects.ulp vbot; | [format-justify-left.png] Align left: Run align_objects.ulp hleft; | [format-justify-center.png] Align center horizontally: Run align_objects.ulp hcenter; | [format-justify-right.png] Align right : Run align_objects.ulp hright;}"*

Icons are from the Tango icon theme

toggle_brd_sch.ulp
=============
Running this ULP will toggle between the board and schematic editor.
You can assign the 'RUN toggle_brd_sch;' command to a shortcut. (I prefer Ctrl+E to get similar behaviour to NI LabVIEW)