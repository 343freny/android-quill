# Frequently Asked Questions #


## Export to Evernote Does Not Work ##

Exporting to Evernote uses the Evernote android app to handle your login data and upload notes. If you have not yet installed the Evernote app you can [download it from the Android market](https://market.android.com/details?id=com.evernote).

## Delete a Notebook ##

To delete a notebook, long-press on the notebook and select **delete**.

In more detail:
  * From the main screen, press the Quill icon on the top left to go to the page overview.
  * Select **Switch notebook**.
  * In the list all notebooks, touch and hold the notebook you want to delete.
  * Press the **Delete** button.
  * Confirm with **Yes** that you really want to delete the notebook.


## Delete a Tag ##

First, note that unused tags are deleted automatically after a while. If you can't wait (or don't want to remove the tag from all pages where it is used) you can explicitly delete a tag from the tag screen by long-pressing the tag and clearing the tag name.

In more detail:
  * From the main screen, press the **Tags** button on the top left to go to the tags screen.
  * In the vertical column on the left, touch and hold the tag that you want to delete.
  * The _Edit tag_ dialog appears; Erase the tag name.
  * Press **OK** to confirm.

## Restore a Notebook Backup ##

Go to **Settings** -> **Restore backup**. The .quill file must be in the root directory of the internal "sdcard" / external (actual) sdcard. Need to write a file browser some day ;-)


## Not Downloading from Market ##

Since I am not operating the Android Market, there is unfortunately little I can do. However, so far any problems with downloads have resolved themselves very quickly. Usually the download starts immediately, but if it doesn't then give it a day or so.

Here is a workaround that sometimes helps:
  * Go to the Android market
  * Go to "My Apps"
  * Under the apps list, there should be Quill under "Not installed".
  * Manually click on install!

If this does not fix your issue then you might want to contact the [Android market support](http://support.google.com/androidmarket/bin/request.py?hl=en&policy=apps&contact_type=contact_policy) directly.

## Input Preferences are Grayed Out and Unselectable ##

Some input preferences are only available if your Android device has hardware pen support. See [Stylus support](StylusSupport.md) for details about different stylus technologies that are supported in Quill. Only devices with hardware stylus support is can distinguish pen and finger input. This is why **Pen Input Mode** and gestures are grayed out in devices without such hardware support.

## How To Convert the .quill File Format ##

There is a desktop companion program at https://github.com/vbraun/QuillDesktop to view Quill notebooks and convert them into svg, pdf, ps. It is written in Python/GTK and should run on pretty much any platform (Windows/Mac/Linux/**nix). Its not feature-complete yet but will be improved over time.**

Thanks to Nicholas A. Knouf (https://github.com/zeitkunst/quill_utils) whose script I used for my program.