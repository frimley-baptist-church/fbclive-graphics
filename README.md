# fbclive-graphics-feed

An Ubuntu configuration package to run the FBCLive Graphics system.

The graphics system provides lower 3rd graphics for broadcasts on the [FBC Live YouTube channel](https://www.youtube.com/channel/UCPb62fbC7uBtisUjU__I47g).

This package configures, in our case, a PC (Intel NUC in our case) running Ubuntu Server 20.04 and the Chromium web browser. When powered up, the NUC automatically logs in as the `fbclive` user, runs Chromium in kiosk mode with its home page set to a page on our internal graphics server. The web page itself presents a green background, with lower 3rd items placed on the page.

A Blackmagic ATEM vision mixer takes the HDMI out from the NUC and composits the signal over cameras to present the final image.

Here's an example from the HDMI out.

![Screenshot from 2021-11-06 14-14-14](https://user-images.githubusercontent.com/5892030/140614163-fe650afb-79fd-4361-a958-88be0560fca6.png)


And here is the finished composition once the Atem upstream keyer has done its work.

![fbclive-graphics-example](https://user-images.githubusercontent.com/5892030/140613844-d92f1f4b-fe8c-42d3-bc6b-70d29e2cba64.png)

