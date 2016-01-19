# Quill Manual #

## The Main Screen ##

### Tools ###

Depending on your device's screen resolution, the tools are either shown as icons in the top bar or moved into the menu if there is not enough space.

| **Icon** | **Menu text** | **Description** |
|:---------|:--------------|:----------------|
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_quill.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_quill.png)  | [Fountain Pen](Manual#Fountain_Pen.md) | Pressure-sensitive pen<br />Only visible if your tablet reports pressure |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_pencil.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_pencil.png) | [Pencil](Manual#Pencil.md) | Constant-thickness pen |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_resize.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_resize.png)   | [Move / Zoom](Manual#Move_/_Zoom.md)  | Move paper or zoom into |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_eraser.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_eraser.png) | [Erase](Manual#Erase.md) | Erase pen strokes or other graphics |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_prev.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_prev.png) | [Previous page](Manual#Previous_page.md) | Switch to the previous page |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_next.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_next.png) | [Next page](Manual#Previous_page.md) | Switch to the next page |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_undo.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_undo.png) | [Undo](Manual#Undo.md) | Undo last change |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_redo.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_redo.png) | [Redo](Manual#Redo.md) | Re-apply an what you just undid |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_line.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_line.png) | [Straight Line](Manual#Straight_Line.md) | Draw a straight line |
| ![http://wiki.android-quill.googlecode.com/hg/images/ic_menu_photo.png](http://wiki.android-quill.googlecode.com/hg/images/ic_menu_photo.png) | [Image](Manual#Image.md) | Insert an image |
| ![http://wiki.android-quill.googlecode.com/hg/images/pen_style_history.png](http://wiki.android-quill.googlecode.com/hg/images/pen_style_history.png) | [Pen style history](Manual#Pen_History.md) | Cycle between the last 10 pen/color/thickness combinations |


#### Fountain Pen ####

Depending on how much pressure you exert, this pen's line thickness will vary. Note that this requires an active digitizer to register the pen pressure (ThinkPad Tablet, HTC Flyer, HTC Jetstream). If you have a capacitive pen (round, thick tip) then there is no pressure sensor and, sadly, the line thickness will not vary.

Gestures (may be disabled in the settings):
  * Double tap switches between full screen and full width. The first double tap switches to full screen. Subsequent double taps toggle between full width and full screen.
    * Full screen lets you see the whole page.
    * Full width fills the whole width of the screen.
  * **Two-finger gesture**: If you touch the screen with two fingers that are **at least half of the screen width apart**, then you can move the paper without disturbing the current zoom setting.

#### Pencil ####

This pen writes with constant thickness, ignoring the pressure.

Gestures are the same as in the [Fountain Pen](Manual#Fountain_Pen.md) mode described above.

#### Move / Zoom ####

This lets you move around and freely zoom into the screen. There is no difference between finger touches and pen input:
  * If you touch the screen with a single finger, you can drag the paper around.
  * Two fingers let you pinch-to-zoom: as you vary the distance between the fingers you can zoom in and out of the paper. This is similar to the Google Maps application, just with paper instead of a map.

#### Erase ####

Anything you touch on screen disappears. No distinction is made between finger and pen input. If you delete something accidentally, use the [Undo](Manual#Undo.md) button to bring it back.

#### Previous page ####

Switch to the previous page matching the tag filter.

#### Next page ####

Switch to the next page matching the tag filter. If you are on the last page, a new page is automatically inserted with the same tags.

#### Undo ####

Reverts the last change that you made.

#### Redo ####

After you used [Manual:Undo Undo], this lets you apply the (previously undone) change again.


#### Straight Line ####

Draw a straight line, or manipulate the endpoints of straight lines.


#### Image ####

Use the image tool to insert an image, or to modify existing images. To insert a new image, simply draw a rectangle. The empty rectangle will be shown in green outlines while you draw it. When you let go of the pen, the image selection screen appears and lets you take a photo or pick an existing image.

To move / resize an existing image, drag the red corner control points to the desired location.

To change an existing image to a different image, drag the image to the "Gears" icon at the bottom left.

To erase an existing image, drag the image to the "trashcan" icon at the bottom right.


#### Pen History ####

The last 10 different pen/color/tickness combinations are remembered. You can cycle through them by repeatedly touching the currently active pen style, or by directly picking one from the history.

Currently there is no way to customize the pen style history. Just use the pen styles that you like and the last 10 will be in the history.

## Tags ##

Each page can be marked by tags. The tags will be shown in fine print on the bottom right of the screen (but do not appear if you export the page).


## Thumbnail Overview ##

You can restrict the yourself to a subset of the pages of the notebook by selecting tags in the left column. Then only pages that are tagged with these tags are shown.




## Frequently Asked Questions ##

  * [Export to Evernote Does Not Work](FAQ#Export_to_Evernote_Does_Not_Work.md)
  * [Delete a Notebook](FAQ#Delete_a_Notebook.md)
  * [Delete a Tag](FAQ#Delete_a_Tag.md)
  * [Not Downloading from Market](FAQ#Not_Downloading_from_Market.md)
  * [Input Preferences are Grayed Out and Unselectable In the Settings Screen](FAQ#Input_Preferences_are_Grayed_Out_and_Unselectable.md)
  * [How To Convert the .quill File Format](FAQ#How_To_Convert_the_.quill_File_Format.md)