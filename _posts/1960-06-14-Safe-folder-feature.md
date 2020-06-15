---
layout: post
title:  "Files by Google preparing to offer encrypted folder called ‘Safe folder’:"
author: mohit
categories: [Tech]
image: assets/images/google/files-by-google.png
tags: [Google, Android, Files by google ,]
---

Google, has been trying to keep privacy as one of its key goals and we can find hints of it in the Android 11 Beta, In which Google has removed the option for allowing apps to take data from phones always.

<a href="{{site.baseurl}}/assets/images/google/files-by-google/xda-safe-folder-intro.jpg" data-lightbox="image-1" data-title="My caption"><img width="20%" src="{{site.baseurl}}/assets/images/google/files-by-google/xda-safe-folder-intro.jpg"></a>
<a href="{{site.baseurl}}/assets/images/google/files-by-google/xda-safe-folder-moving.jpg" data-lightbox="image-1" data-title="My caption"><img width="20%" src="{{site.baseurl}}/assets/images/google/files-by-google/xda-safe-folder-moving.jpg"></a>
<a href="{{site.baseurl}}/assets/images/google/files-by-google/xda-safe-folder-remember-password.jpg" data-lightbox="image-1" data-title="My caption"><img width="20%" src="{{site.baseurl}}/assets/images/google/files-by-google/xda-safe-folder-remember-password.jpg"></a>

In the decompiled latest version of the Files by Google, `9 TO 5 Google` was able to find this feature. They found that they have added a new feature called the **Safe folder**, where users can safely hide their files and keeps them from being accessed by other apps or by anyone other than you who has access to your phone. The authentication for this will be done by Pin. We think Google might end up adding fingerprint and face unlock before the official release of this feature.

If you see the code below, We cannot find any built-in methods to recover password, If you happen to forget the password, While nothing states that your files are being encrypted, the fact that Files by Google can’t recover the files or password strongly suggests **encryption is involved**.

No surprise to see Google to make such a move since most of the users are losing confidence from Google in terms of privacy, Samsung has been offering the same feature for years in their phone and called it Secure Folder.

<<<<<<< HEAD
Below is the code found by 9 TO 5 Google. 
```java
=======
Below is the snipets of the code found by 9 TO 5 Google.

>>>>>>> ac766c06bf7232144b5ee727fcb552711a411da0
<string name=”safe_folder_label”>Safe folder</string>
<string name=”safe_folder_first_time_tooltip”>Move any files you want to keep protected by a PIN to this folder.</string>
<string name=”safe_folder_after_setup_tooltip”>Find your protected files in this folder.</string>
<string name=”remember_your_password_warning_title”>Remember your password</string>
<string name=”remember_your_password_warning_description”>”Safe folder can’t be opened again if you forget the password.”</string>
<string name=”remember_your_password_warning_button”>Got it</string>
<string name=”move_into_safe_folder_menu_text”>Move to Safe folder</string>
<string name=”move_out_of_safe_folder_menu_text”>Move out of Safe folder</string>
<string name=”confirm_pin_to_move_title”>Confirm PIN to move</string>
```