# Explanation of Requested Permissions #

I'm of course trying to use the minimal amount of permissions, but not at the expense of safety or user friendliness. Having said that, here is the list of permissions that the Quill APK requests in order to function.


## Full Internet Access ##

  * Market description: _Allows the app to create network sockets._
  * Code: **`android.permission.INTERNET`**

This permission is required to sync your notebook online, if you chose to. Note that nothing is sent or received over the internet unless you create a Quill account.


## Act as an Account Authenticator ##

  * Market description: _Allows the app to use the account authenticator capabilities of the AccountManager, including creating accounts and getting and setting their passwords_
  * Code: **`android.permission.AUTHENTICATE_ACCOUNTS`**
  * Code: **`android.permission.GET_ACCOUNTS`**

This permission allows Quill to create and display an account in the Android preferences. Also, allows Quill to get/set the password for Quill's own account

<p align='center'>
<img src='http://wiki.android-quill.googlecode.com/hg/images/show_account.png' />
</p>

The market description is a bit terse, but note that the _their_ in _getting and setting their passwords_ refers to the account that the app created. There is no permission in Android that would allow an app to access **other** app's passwords.


## Read Contact Data ##

  * Market description: _Allows the app to read all of the contact (address) data stored on your tablet. Malicious apps may use this to send your data to other people. Allows the app to read all of the contact (address) data stored on your phone. Malicious apps may use this to send your data to other people._
  * Code: **`android.permission.READ_PROFILE`**
  * Code: **`android.permission.READ_CONTACTS`**

This permission is used to read your own profile, so you do not have to type your own name and email if you want to create a Quill account. Note that your profile information is only used to provide defaults for your name and email when creating an account, and you can change them arbitrarily before creating an account:

<p align='center'>
<img src='http://wiki.android-quill.googlecode.com/hg/images/create_account.png' />
</p>

Unfortunately there is no finer-grained permission to only let an app access your own profile but not other contacts. Hopefully this will be introduced in a future Android version. If you want to verify for yourself that Quill only queries your own profile data, you can look into [UserProfileICS.java](http://code.google.com/p/android-quill/source/browse/src/com/write/Quill/sync/UserProfileICS.java) in the Quill sources:
```
private void initialize(Activity activity) {
    ContentResolver cr = activity.getContentResolver();
    Uri profile_uri = Uri.withAppendedPath(
                ContactsContract.Profile.CONTENT_URI,
                ContactsContract.Contacts.Data.CONTENT_DIRECTORY);             
    Cursor cursor;
    cursor = cr.query(profile_uri, QueryEmail.PROJECTION,
                      QueryEmail.SELECTION, QueryEmail.ARGS, null);
```
Quill queries `ContactsContract.Profile.CONTENT_URI`, so only the user's own profile information is returned.


## Modify/Delete USB Storage Contents, Modify/Delete SD Card Contents ##

  * Market description: _Allows the app to write to the USB storage. Allows the app to write to the SD card._
  * Code: **`android.permission.WRITE_EXTERNAL_STORAGE`**

This is required in order to save backups and/or PNG/PDF exported files.