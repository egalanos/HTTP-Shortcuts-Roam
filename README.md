# HTTP-Shortcuts Roam Quick Capture

This is a shortcut for the Android app [HTTP Shortcuts](https://http-shortcuts.rmy.ch/)
 to provide an alternative Quick Capture method for [Roam](https://roamresearch.com/).

## Differences from the Quick Capture feature in the Roam mobile app

 * Faster single step capture process
 * Can be triggered with an Android widget or Quick Settings Tile
 * Can automatically add a suffix to captured blocks (for example, `#inbox`)
 * Destination can be configured to today's Daily Note page, a page, or under a block ref

## Limitations

 * Only supports a single graph
 * Won't work on encrypted graphs
 * It does not work offline or retry in case of failure
 * Just a simple plain text save

# Setup instructions

## On your Android device
 1. Install **HTTP Request Shortcuts** from the [Google Play Store](https://play.google.com/store/apps/details?id=ch.rmy.android.http_shortcuts)


 1. Import shortcut by tapping this [Android deeplink](<http-shortcuts://import?url=https%3A%2F%2Fgithub.com%2Fegalanos%2FHTTP-Shortcuts-Roam%2Freleases%2Flatest%2Fdownload%2Fshortcuts-roam.zip>)
    , or manually:

     1. Download [shortcuts-roam.zip](https://github.com/egalanos/HTTP-Shortcuts-Roam/releases/latest/download/shortcuts-roam.zip)

     1. Open the HTTP Shortcuts app

         1. Tap the options menu (three vertical dots), then `Import / Export`, 
         then `Import from File`

         1. Select the downloaded file

 1. Enter your Roam graph settings:

    1. Tap the `Roam Graph Settings` shortcut

    1. Enter your graph name

    1. Enter your graph token. To create a new graph token:

         1. Log in to Roam at https://relemma-git-feat-frontdesk.roamresearch.com/
             * NB: The interface to manage graph API tokens is not in the
               standard Roam web and desktop apps at the time of writing. See
               [Roam Backend API](https://roamresearch.com/#/app/developer-documentation/page/W4Po8pcHQ)
               for further details

         1. Open your graph, then select the full site version

         1. Tap on the `Share, export, and more` menu (three horizontal dots top right),
            then `Settings`, and then `Graph`

         1. Tap `+ New API Token`
            * Descriptor: `HTTP Shortcuts`
            * Access Scope: **edit access**
            * Tap `Create`

         1. Copy the token, then switch back to the HTTP Shortcuts app and paste it 

    1. Follow the remaining prompts

    The shortcut will verify that the graph API settings are correct

 1. Tap `Roam Quick Capture` to use it!
    * Tip: You can also share text into it from other apps using the standard Android
      share mechanism

 1. (Optional) Add a widget to your home screen using the standard Android touch
    and hold and select `Widgets`, etc
