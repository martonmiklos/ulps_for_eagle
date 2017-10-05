Various ULPs (User Language Programs) for the Cadsoft EAGLE
=============


selection_to_variant.ulp
=============
This ULP can be used to add/remove selectd parts to/from a selected Assembly variant.

* Usage: select parts
* Run ULP
* Select the action and the board variant
* Click Ok

![selection_to_variant](https://raw.githubusercontent.com/martonmiklos/ulps_for_eagle/master/screenshots/selection_to_variant.png "selection_to_variant.ulp in action")

show_values.ulp
=============
This ULP was originally written by Karsten Brandt.
Following features were added:
* Command line argument handling: RUN show_values 100n {top,bottom}
* Ability to display parts only on top/bottom side

![show_values_screenshot](https://raw.githubusercontent.com/martonmiklos/ulps_for_eagle/master/screenshots/show_values.png "show_values.ulp in action")

toggle_brd_sch.ulp
=============
Running this ULP will toggle between the board and schematic editor.
You can assign the 'RUN toggle_brd_sch;' command to a shortcut. (I prefer Ctrl+E to get similar behaviour to NI LabVIEW)

add_name_and_value_lbr.ulp
=============
This ULP can be used to place the >NAME and >VALUE in the symbol and footprint editor. 

Add the following to your .eaglerc:
```
Lbr.MenuText.<whatever is your last menu index + 1> = "Place labels: RUN add_name_and_value_lbr.ulp;"
```
