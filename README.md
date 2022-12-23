# Self updating Wahoo Bolt VTM themes

This repo is a continuation of [a gist I
made](https://gist.github.com/BadmanBarista/47c34b5e9dca3910bba89c4bcdeb58b6)
over a year ago. Turns out Wahoo update their VTM themes from time to time and
adds new things, so the VTM themes I created then no-longer work now.

To solve this issue, this repository will automatically check for wahoo updates
every sunday at midnight and recreate the themes if it finds one.

I can't guarentee that it'll work forever as it's just using `sed` to replace
the lines and values necessary. If Wahoo ever changes those names, or moves the
default vtm theme, then this process will break.

If you notice any issues or problems with the resultant themes, [please open an issue here!](https://github.com/BadmanBarista/wahoo-vtm-themer/issues/new/choose)

Feel free to use this repository as a template for creating your own auto
updating themes. You will want to change the `user.name` and `user.email` in
`.github/workflows/auto_update.yml`, and perhaps use a better tool than `sed`
for your theme changes.

## Using the themes

There are two themes, HIDDEN, and THIN. The former will hide blue cyclepaths
completely. The latter will make them very thin.

1. Download your prefered XML theme from [the most recient release](https://github.com/BadmanBarista/wahoo-vtm-themer/releases/latest).
2. Rename it to `vtm-elemnt.xml`.
3. Turn on your Bolt v2.
   Plug it into a PC that supports MTP (Windows does out the box, [More info can be found here](https://support.wahoofitness.com/hc/en-us/articles/115000127910-Connecting-ELEMNT-BOLT-ROAM-to-Desktop-or-Laptop-Computers)).
4. Open the Bolt's internal storage.
5. Open the maps folder.
6. Create a new folder call vtm-elemnt.
7. Copy your `vtm-elemnt.xml` into the folder.
8. Reboot your Bolt v2.
