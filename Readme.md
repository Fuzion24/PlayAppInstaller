#PlayAppInstaller

It is a demonstration application that indicates that you can install any app from the play store with root privileges without.

This app does not have only the permissions of the following three, since it can be made to install any app of play store, for example, play store the app that has the function of transmitting to the net by reading the contact It is possible to be installed from. And, it will be able to start the application immediately after installation, such as that steal contacts.

However, since there is a way to prevent the installation of this technique by PlayAppInstaller, please read the description of the following means.

#### Apology

After you have installed from the play store, that app was tweeted to be able to launch itself automatically in tweets August 29 midnight, but it seems to no longer be such a thing in Android 3.1 or later? Sorry, could not and would to disseminate false information. However, apps you have installed, so can be launched from this app, it is possible real, equivalent.

### Download

* [PlayAppInstaller.apk](https://github.com/downloads/virifi/PlayAppInstaller/PlayAppInstaller.apk)


### Permissions

* android.permission.INTERNET
* android.permission.GET_ACCOUNTS
* android.permission.USE_CREDENTIALS

### ScreenShot

![スクリーンショット](https://raw.github.com/virifi/PlayAppInstaller/master/readme_imgs/screenshot1.png)

### License

```
 Copyright (C) 2012 virifi

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 ```

### Commentary

#### Operating conditions of this app

This app allows you to install any app of play store, but there is always a necessary condition in order to perform the installation process. It, when you start the installation process, a screen similar to the screen shot on the left I see, but you need to push the user to "Allow Access" on this screen. As long as the user does not press the "Allow Access", you can not run the installation process.

#### What happens if you allow access

Access token so that you can press the permission of access, log in to the Web version play store through AccountManager is issued. By using this access token, you will be able to without entering a password and user name of the account of Google users, to log in to play store.

Also, after logging in to play store, site will be displayed while logged continue to load the site of Google Calendar and GMail, it is possible to read steal and appointments mail.

You will learn below, but it is also to forgive any permission for this app substantially.

#### Do you have installed the app How do I

Installation There are buttons on the page for each app play store for the Web version. When you press this button installation, you can install the app on the remote terminal. Also, play store for the Web version will work correctly when viewed in WebView in Android.

You have realized the installation process by automating the process by using the WebView, log in to play store in the user's account first, open the page of the application you want to install, and press the Install button in this app.

#### Risk of that would have been installed any app

If you want to read, such as contacts, the operation sensitive, you need to grant permissions to apps apps Android. And, when you install the app, users will be able to install it to confirm that app is whether to request what kind of permission.

If you do not have the required permission of the reading of the contacts, I do not have to worry about is read a contact by that app.

However, to be able to be made to start to install any app, to forcibly installs without user consent the app that have permission contact reading, is allowed to start automatically, that is sent to the net contact It's easy can be like.

In other words, in the original, it has not only requires permission of one 3 INTERNET, GET_ACCOUNTS, of USE_CREDENTIALS, but it should not have to worry about is read a contact, by using this technique, the safety'm gone bankrupt .

By allowing the user pressed the "Allow Access" permissions and the three, this app is a good as the apps that have been granted the permission of any.
 
#### Description of PlayAppInstaller

When you press the install button is allowed to launch this app, from the play store AutoStartApp and then install. After installation, I will activate automatically AutoStartApp.

AutoStartApp is an app only to display the status of the current wifi. You must android.permission.ACCESS_WIFI_STATE has been granted to the app to get the status of the wifi. Of course, AutoStartApp you have it.

However, PlayAppInstaller does not have that permission. Therefore, you can not realize that that is displayed on the screen to get the state of the wifi it would otherwise. However, by using the techniques described above, it has got realized.

[AutoStartApp](https://play.google.com/store/apps/details?id=net.virifi.android.autostartapp)

#### CounterMeasure

Like the image above, please refuse When you are prompted to authority that contains the string beginning at google "weblogin". This request will be displayed when you first get the access token, but you can get an access token without through this screen later it has been fully permitted once. Therefore, even if you do not do anything when you press the permission of access, we are able to perform an illegal operation one month after you press.

If you've allowed if, https://accounts.google.com/b/0/IssuedAuthSubTokens Please revoke permissions on this page.


#### Note

Application to request the permission of access, such as described above should not mean doing the incorrect behavior necessarily. However, the fact that installing the apps like that, you should install considered equivalent to that are going to install an app that has all the permissions that Android has defined.

I'm not supposed to install if, when there is apps like to request all permissions. If you do not know this technique, with it you might had gotten done before I knew that equivalent.

I put it in my head all means that you have said this, let's use more secure Android.
