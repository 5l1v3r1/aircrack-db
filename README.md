# aircrack-db

aircrack-db is a list of wireless interfaces tested with the dual-card injection test and in the field.

The driver name is the name of the kernel module used by the card. The driver version is either the kernel version or the version of the [compat-wireless / compat-drivers / backports](https://backports.wiki.kernel.org/index.php/Main_Page) drivers if they were installed separately. All of the used drivers are mac80211 drivers. The hardware vendors usually don't bother to implement monitoring mode in their drivers. A common example is the wl driver from Broadcom.

Aircrack-ng's wiki page about [injection testing](http://www.aircrack-ng.org/doku.php?id=injection_test) states:

> If you get a failure on attack 5, it may still work in the field if the injection MAC address matches the current card MAC address. With some drivers, it will fail if they are not the same.

If the wireless interface proves to work in my lab for the fragmentation attack, then it is going to be mentioned in a separate column. I use Kali Linux 1.0.9 and Aircrack-ng 1.2-beta3 for gatherting this information.

Due to the fact that GitHub uses "toiler paper design", hence I can't fit a table without having a horizontal scroll, even on a FullHD screen, the information about the hardware is [here](http://saltwaterc.github.io/aircrack-db).

The contributions to this project are accepted. Just send a pull request / patch for db.json. This is the file that contains the details about the hardware.
