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
 1. Install **HTTP Request Shortcuts**[^1] from the [Google Play Store](https://play.google.com/store/apps/details?id=ch.rmy.android.http_shortcuts)

 1. Import shortcut automatically with this [Android deep link](https://tinyurl.com/5dhe5c2r)
     <details><summary><sup>(show manual instructions)</sup></summary>

     1. Download [shortcuts-roam.zip](https://github.com/egalanos/HTTP-Shortcuts-Roam/releases/latest/download/shortcuts-roam.zip)

     1. Open the HTTP Shortcuts app

         1. Tap the options menu (three vertical dots), then `Import / Export`, 
         then `Import from File`

         1. Select the downloaded file
      </details>

     then tap the back arrow to get to the app main screen

 1. Create a Roam graph API token

    1. Log in to Roam in a new browser tab at https://relemma-git-feat-frontdesk.roamresearch.com/ [^2]

    1. Open your graph, then select the *Full site* version (top right corner)

    1. Tap the `Share, export, and more` menu (three horizontal dots top right),
       then `Settings`, and then `Graph`

    1. Tap `+ New API Token`

       |Descriptor|Access Scope|
       |----------|------------|
       | `HTTP Shortcuts` | **edit access** |
       * Tap `Create`

     1. Copy the token, then switch back to the HTTP Shortcuts app

 1. Tap the `Roam graph settings` shortcut:

    1. Enter your graph name

    1. Enter your graph token

    1. Follow the remaining prompts

    The shortcut will verify that your graph API settings are correct

 1. Tap `Roam Quick Capture` to use it!
    * :bulb: Tip: You can also share text into it from other apps using the standard Android
      share mechanism

 1. (Optional) Add a widget to your home screen using the standard Android touch
    and hold and select `Widgets`, etc


[^1]: The app name will be **HTTP Shortcuts** once installed

[^2]: The interface to manage graph API tokens is not in the standard Roam web and desktop apps at the
      time of writing. See [Roam Backend API](https://roamresearch.com/#/app/developer-documentation/page/W4Po8pcHQ)
      for further details
