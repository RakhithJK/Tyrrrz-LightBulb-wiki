LightBulb's main goal is to reduce the eye strain from staring at your monitor during late hours. It has similar functionality to Windows 10 built-in "Night Light" feature, as well as to some other apps like F.lux, Iris, SunsetScreen, but offers additional features and better customization.

As the day goes, the illumination in our surrounding environment changes. During day-time, our main source of light is the sun, which emits a bright white light. During the evening and night-time, after the sun sets, we resort to artificial light, typically incandescent or fluorescent light bulbs, which have a slight yellowish tint.

The "color" we associate with different light sources is measured by a value called [**color temperature**](https://en.wikipedia.org/wiki/Color_temperature).

![different color temperature](https://i.imgur.com/LeQm9iM.png)

Almost all displays are calibrated to match the color temperature of around 6500-6600 degrees Kelvin, which looks fine during day-time, but is excruciating at night. Most people don't notice this because their eyes get used to it after a while, but staring at a bright monitor at night is actually pretty bad for your eyes.

Ever had issues with your eyes getting too sore, your head aching or having trouble falling asleep after working late hours behind your computer? It's not unlikely that reducing blue light may help with that.

What LightBulb does is that it gradually changes the gamma of your monitor, starting at sunset, matching the color temperature and brightness settings you have configured. As long as the configuration matches your surrounding environment, your monitor will emit the same type of light as the artificial light in your room, reducing eye-strain and making it easier to fall asleep.

## LightBulb dashboard

The main screen you will see when you launch LightBulb is the so-called dashboard. It shows the sundial and some relevant information.

![dashboard](https://i.imgur.com/5AlA3zz.png)

Here you can see the whole day cycle represented using a circle partitioned in 3 phases: day phase, night phase, and transition phase. In the middle it shows the current state, color temperature, brightness, and time. On the circle itself you will find a smaller moving orange circle that represents your current "position" within the cycle.

## Configuring LightBulb

LightBulb comes with a lot of different settings, but first thing you should do is ensure it uses your correct location. To get the most out of this application you will want it to automatically calculate sunrise and sunset based on where you live.

### Set your location

1. Open **Settings** and navigate to **Location settings** by clicking on the globe icon on the left.

![go to location settings](https://i.imgur.com/q7rHaQd.png)

2. Under **Solar configuration** select **Location-based**.

![select location-based](https://i.imgur.com/HnirJXg.png)

3. Here you can either auto-detect your location based on IP using the ![autodetect button](https://i.imgur.com/tiMDJGA.png) button on the left or type in an address or raw coordinates and press the ![set location button](https://i.imgur.com/rPRJO6J.png) button.

![manual location using search query](https://i.imgur.com/rX298oZ.png)

4. After that, LightBulb should get the correct coordinates and use that location to calculate sunrise and sunset going forward. Click **Save** to commit your changes.

![location is set](https://i.imgur.com/JtoV2Bm.png)

### Set your desired temperature and brightness settings

LightBulb comes with default settings of 3900K / 80% for night time which will look fine on most monitors. That said, different monitors (and GPUs) have different color profiles, so you will really want to fine-tune this values to your liking. The same color configuration in LightBulb may look completely differently on different monitors.

1. Open **Settings** and navigate to the first tab, **General settings**.

![general settings](https://i.imgur.com/sf0TrF4.png)

2. Move the corresponding sliders to match your desired settings. Your monitor may not be affected, depending on the current time of day. It's recommended to wait until the sun sets so that you can calibrate LightBulb against the actual light you have in your room during night-time.