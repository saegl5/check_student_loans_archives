# ![Alt](./app_icon_and_logo.png "Check Student Loans"): Archives

This project consists of collection of resources of an experimental study.

## Instructions

Download the respective ZIP file, and <i>unzip</i> it.

Open the IPYNB file with SageMath Notebook.<br>
Open the XLSX file with Microsoft Excel.<br>
Open the DOCX file with Microsoft Word.<br>
Open the URL file with Microsoft (Chromium) Edge in Windows. The extension may be hidden.<br>
Open the WEBLOC file with Safari in macOS.<br>
Open the DESKTOP file with Mozilla Firefox in Ubuntu.<br>
Open each PDF file with [Acrobat Reader DC](https://acrobat.adobe.com/us/en/acrobat/pdf-reader.html "Click here to access the download link.").<br>
Open the TXT file with a text editor (e.g., Notepad, TextEdit or gedit).

The APK file is for Android phones running Android 4.2 (Jelly Bean) or above. 
In security settings, allow installation of apps from unknown sources. Then, install the file directly on Android phones.<br>
The IPA file is for iPhone devices. 
Install the file using iTunes or Apple Configurator on iPhone devices.

Instructional App = course material + Android/iOS app

## Verification

Prerequisites: gnupg (https://www.gnupg.org/)

To verify the authenticity of the files in a terminal:
<pre>
gpg --keyserver hkps://keyserver.ubuntu.com:443 --recv-keys 0x4191f431
gpg --verify SHA1SUMS.gpg SHA1SUMS
</pre>

To verify the integrity of the files in a terminal:
<pre>
(Ubuntu) sha1sum -c SHA1SUMS
(macOS) shasum -a 1 -c SHA1SUMS

(Windows)
ls *.zip | Get-FileHash -Algorithm SHA1
Get-Content .\SHA1SUMS
(check that hashes match)
</pre>

## Notes

If one verifies authenticity using Windows Subsystem for Linux, the terminal may output ``BAD signature.''<br>
Convert file hashes/checksums to Unix format, and retry:
<pre>
sudo apt install dos2unix
dos2unix SHA1SUMS
gpg --verify SHA1SUMS.gpg SHA1SUMS
</pre>

panel_discussion.ipa is a close replica of the native app utilized in the study.<br>
Exceptions are that rounding and interest computations are corrected, and the monthly balance table is restructured.

informal_field_test.apk and focus_groups.apk are identical<br>
panel_discussion.ipa and summative.ipa are identical

## License

Native apps are licensed under the MIT License:
https://opensource.org/licenses/MIT.

Course material and other resources are licensed under the Attribution 4.0 International License: http://creativecommons.org/licenses/by/4.0.