## Usage
1. [Install Automagic **v1.37**](https://automagic4android.com/download_en.html) (no longer maintained, but now free and works great)
2. Download [darktide_automagic_shop_notifications.xml](https://raw.githubusercontent.com/ronvoluted/dt-automagic/main/darktide_automagic_shop_notifications.xml) to your phone and select "Import Flows/Widgets" in Automagic to load it
3. On desktop, inspect the network request for [`atoma.cloud/queue/refresh`](https://accounts.atoma.cloud) and copy the `RefreshToken` value
4. Back in Automagic, hit the 3-dot menu button on "Atoma Activate" and "Execute", then paste in the token from above
5. Follow the prompts to select the Operatives and base level threshold you want!

## Notifications

- Every hour, if any items in the shop for your selected characters meet that threshold, you'll get a notification:

<img width="250" alt="image" src="https://user-images.githubusercontent.com/5785323/210496789-e99a904d-e570-4ab6-b03e-4b5b5b236e3c.png">


- Tap "View summary" to see all items:

<img width="250" alt="image" src="https://user-images.githubusercontent.com/5785323/210496778-91424267-5cd8-4e24-bade-466fd16230ef.png">

- To change the Operatives you want notifcations for or the item level threshold, just Execute "Atoma Activate" again. The current `RefreshToken` will already be in place so you don't need to copy it a second time (unless something goes wrong)
- Execute "Atoma Show" to display the latest summary again
- By default you will get notifications beteen 8AM and 11PM. You can edit this in "Atoma Check" inside the first node, "Periodic Timer"


## How to find refreshToken via Inspect tool with Firefox/Chrome

1. Go to [`atoma.cloud/queue/refresh`](https://accounts.atoma.cloud) and login.
2. Press F12, Under "Network" tab, hit reload ![image](https://user-images.githubusercontent.com/64565597/210626250-9fb60faa-4778-4e29-967f-853d58dcaa0a.png)
3. Find under the column "File" for "refresh"![image](https://user-images.githubusercontent.com/64565597/210626476-3d3e3db3-63a2-416f-8e32-755e7094098d.png)
4. To the right sidebar, click on "Response", here you will see the refresh token ![image](https://user-images.githubusercontent.com/64565597/210626614-4581c743-1014-469b-bf31-6bfb79067ee4.png)

## FAQ
### Can I run this on an android emulator? YES!

1. Download https://www.bluestacks.com/
2. Drag and drop "Automagic" into the emulator
3. Import [darktide_automagic_shop_notifications.xml](https://raw.githubusercontent.com/ronvoluted/dt-automagic/main/darktide_automagic_shop_notifications.xml) from OS drive

### What is the best time setting for a 24hr check?

You can make this work with any hrs as long as it doesn't overlap the "From" time 
![image](https://user-images.githubusercontent.com/64565597/210627369-a7530395-c1d2-4eaf-8e72-9d85ccf2a184.png)

### Are there other options/features?

Yes, in "Atoma Check" you can check the boxes for things features you want ![image](https://user-images.githubusercontent.com/64565597/210627696-ee74e3c7-33f5-4a56-9b0b-381d6e86f304.png)
