> **Warning**
>
> Automagic is not maintained anymore and is no longer available on Google Play. To download it, visit [the site's .apk download page](https://automagic4android.com/download_en.html)

## Usage
1. Install Automagic
2. Download [darktide_automagic_shop_notifications.xml](https://raw.githubusercontent.com/ronvoluted/dt-automagic/main/darktide_automagic_shop_notifications.xml) to your phone
3. In the Automagic menu, select "Import Flows/Widgets" and load the XML file you downloaded
4. Enable the 3 imported scripts:
- Atoma Refresh (used to automatically refresh your access token)
- Atoma Check (used to query the Darktide API, filter it and format the notification summary)
- Atoma Show (used to display the summary from the notification)
5. On desktop, go to https://accounts.atoma.cloud, inspect the network request for `atoma.cloud/queue/refresh` and copy the `RefreshToken` value
6. Open "Atoma Refresh" in Automagic, edit the "Set refresh token" node and replace `YOUR_REFRESH_TOKEN_COPIED_FROM_ATOMA.CLOUD/QUEUE/REFRESH_NETWORK_REQUEST` with the value you just copied.
7. Open Atoma Check, edit the "Select Character" node and replace `YOUR_OPERATIVE_NAME` with one of your character's names
8. Edit the "Parse Store Items" node and edit `360` to whatever minimum base rating of items you want to get notifications for

Every hour, if any items in the shop for your character meet that threshold, you'll get a notification:

<img width="312" alt="image" src="https://user-images.githubusercontent.com/5785323/210309482-e5881f10-76cf-4b1d-b3d2-1a32edc17602.png">

Tap "View summary" to see all items:

<img width="272" alt="image" src="https://user-images.githubusercontent.com/5785323/210309552-e2735159-0a3d-4556-b522-319b9dda01e4.png">

## Maintenance

This was quickly slapped together to get notifications on my phone. Since Automagic has ceased development and other people are working on an atoma.cloud API abstraction, anything else I might do will use different methods.
