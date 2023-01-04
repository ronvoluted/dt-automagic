## Usage
1. [Install Automagic](https://automagic4android.com/download_en.html) (free)
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
