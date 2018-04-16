# Publishing App in Apple Store or Google Play Store.
How to prepare app to be successfully accepted by reviewers

Mostly I published apps build in Ionic(Cordova Webview apps ak. Hybrid). Is more simply when you have to create one app on 2 diffrent system. In my case (iOS and Android never done it on Windows mobile).

But all are the same, screenshots, privacy, content, it's just another way to creating mobile apps using web features.

## Overview

  - [Privacy](#Privacy)
  
  - [Desing](#Desing)

  - [Terms of service or Privacy Policy.](#Terms-of-service-or-Pivacy-Policy)
  
  - [Screenshot, Splash, Icons](#Screenshot-Splash-Icons)
  
  - [HTTPS | HTTP | ENCRYPTION](#HTTPS-HTTP-ENCRYPTION)
 


### Privacy
If your app requests user data or makes sensitive permissions requests such as Phone, Accounts, Contacts, Camera, or Microphone, you’ll need to add a valid privacy policy in two places: your app’s Store Listing page (instructions below) and within your app.

For example it can be "access to gallery of user" it has to have permission and policy(mostly web site where is written what you do with the things and what happen when you have security breach and it can expose user data in this case images). Make sure to descripe what are you doing with the (in this case gallery) do you just save or read? Or maybe you upload to your server. 

here is link to full article about it for goole play store: https://www.iubenda.com/blog/warning-google-play-developer-policy-violation-action-required-policy-issue/


(iOS)***

When you need to access user device by the app. You need to descripe by informations what it will do (saves, reads, writes, modify). Add text bellow to info.plist where Key      :  Privacy - Calendars Usage Description    

Value  :

              This app wants to accces Calendar to save events.
              
This message is clear and inform user that this app just want to save events without acccesing it after or reading informations from your calendar. (Accepted by the reviewers.)

This is just example I wrote it here so I can use it in future.  The same when you use notifications, camera to scan qr codes or get permissions to read/write to gallery of user on device.


### Desing              
App has to act as native never as website. Build app in Webview makes app look like web apps not like native. Always try to do in the way from the smallest to the bigger. Apps doesn't need to have all features in one place hide it. Make user choose what he/she can do with the app. 


### 4.2 Minimum Functionality (ios)  (android***)
Once I sent app where we get informations from the web page of client Apple store Reviewers reject my app because it hasn't any native 
functionality.

In that case you need to add some featuers such as qr scaner for example to add events by the qr codes. Adding to Calender, Sending emails, Storage data on user device, Synchronization, Notifications. 

Of course adding this features you need to have already plan what you will use and what kind of privacy policy it will be look like. 


*** For android I didn't have any problems but in future Play store might add the same thing so keep that in mind.

### Terms of service or Privacy Policy. 

Always try to have both. But don't reapet yourself and keep things clear and divide important things on this two. Otherwise it may cause you problems. 


### Screenshot, Splash, Icons.

Before you publish your app you need to have screenshots to submit for review. 

- For phones and tablets.
- For iphones and ipads.

I will not write here what size etc because those things always changes.

Splash has also dimession you need to have on diffrent screens. Also I can't write what they are now because they change as well.
Always try to have your image, content, text in the middle. 


Ioncs.

- For android it can be transparent.
- For ios it can't be transparent. ( you need to upload one before you send to review).



### HTTPS | HTTP | ENCRYPTION

When you are accessing your server via http protocol and you have login via https you need to have Encryption Registration Number (ERN).
Signing by USA Government where are the stores( apple store and play store).

When you have those files you need to upload them in the stores. There is special section where it's all explained.

link to article how to do it and what it is:
https://medium.com/@cossacklabs/apple-export-regulations-on-crypto-6306380682e1

But when you don't have any encryption and you use http in such app when wou getting data:

On android just check that your app doesn't use encryption is when you creating app on play store.

In iOS put that text bellow in info.plist so when you sent the build the system will not reject your app:

      <key>ITSAppUsesNonExemptEncryption</key><false/>
      








