# PublishingApp
How to prepare app to be successfully accepted by reviewers

Mostly I published apps build in Ionic(Cordova Webview apps ak. Hybrid). Is more simply when you have to create one app on 2 diffrent system. In my case (iOS and Android never done it on Windows mobile).

But all are the same, screenshots, privacy, content, it's just another way to creating mobile apps using web features.

### Privacy
If your app requests user data or makes sensitive permissions requests such as Phone, Accounts, Contacts, Camera, or Microphone, you’ll need to add a valid privacy policy in two places: your app’s Store Listing page (instructions below) and within your app.

For example it can be "access to gallery of user" it has to have permission and policy(mostly web site where is written what you do with the things and what happen when you have security breach and it can expose user data in this case images). Make sure to descripe what are you doing with the (in this case gallery) do you just save or read? Or maybe you upload to your server. 

here is link to full article about it for goole play store: https://www.iubenda.com/blog/warning-google-play-developer-policy-violation-action-required-policy-issue/

              
### Desing              
App has to act as native never as website. Build app in Webview makes app look like web apps not like native. Always try to do in the way from the smallest to the bigger. Apps doesn't need to have all features in one place hide it. Make user choose what he/she can do with the app. 


### 4.2 Minimum Functionality (ios)
Once I sent app where we get informations from the web page of client Apple store Reviewers reject my app because it hasn't any native 
functionality.

In that case you need to add some featuers such as qr scaner for example to add events by the qr codes. Adding to Calender, Sending emails, Storage data on user device, Synchronization, Notifications. 

Of course adding this features you need to have already plan what you will use and what kind of privacy policy it will be look like. 


### Terms of service or Privacy Policy. 

Always try to have both. But don't reapet yourself and keep things clear. Otherwise it may cause you problems. 

