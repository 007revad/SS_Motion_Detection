# <img src="images/SurveillanceStation_64.png" width="40"> SS Motion Detection

<a href="https://github.com/007revad/SS_Motion_Detection/releases"><img src="https://img.shields.io/github/release/007revad/SS_Motion_Detection.svg"></a>
![Badge](https://hitscounter.dev/api/hit?url=https%3A%2F%2Fgithub.com%2F007revad%2FSS_Motion_Detection&label=Visitors&icon=github&color=%23198754&message=&style=flat&tz=Australia%2FSydney)
[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/paypalme/007revad)
[![](https://img.shields.io/static/v1?label=Sponsor&message=%E2%9D%A4&logo=GitHub&color=%23fe8e86)](https://github.com/sponsors/007revad)
[![committers.top badge](https://user-badge.committers.top/australia/007revad.svg)](https://user-badge.committers.top/australia/007revad)

The Surveillance Station icon above is Copyright © 2004-2025 [Synology Inc.](https://kb.synology.com/en-br/DSM/help/DSM/Home/about?version=7)

### Description

Installs older version of Surveillance Station and Advanced Media Extensions so motion detection and HEVC playback are supported.

This script installs Surveillance Station 9.2.0-11289 and Advanced Media Extensions 3.1.0-3005

### Download the script

1. Download the latest version _Source code (zip)_ from https://github.com/007revad/SS_Motion_Detection/releases
2. Save the download zip file to a folder on the Synology.
3. Unzip the zip file.

### To run the script via task scheduler

See [How to run from task scheduler](https://github.com/007revad/SS_Motion_Detection/blob/main/how_to_run_from_scheduler.md)

### To run the script via SSH

[How to enable SSH and login to DSM via SSH](https://kb.synology.com/en-global/DSM/tutorial/How_to_login_to_DSM_with_root_permission_via_SSH_Telnet)

```YAML
sudo -s /volume1/scripts/ss_motion_detection.sh
```

**Note:** Replace /volume1/scripts/ with the path to where the script is located.

### Troubleshooting

If the script won't run check the following:

1. Make sure you download the zip file and unzipped it to a folder on your Synology (not on your computer).
2. If the path to the script contains any spaces you need to enclose the path/scriptname in double quotes:
   ```YAML
   sudo -s "/volume1/my scripts/ss_motion_detection.sh"
   ```
3. Make sure you unpacked the zip or rar file that you downloaded and are trying to run the ss_motion_detection.sh file.
4. Set the script file as executable:
   ```YAML
   sudo chmod +x "/volume1/scripts/ss_motion_detection.sh"
   ```

### After running the script

Enable HEVC decoding:
1. Open Package Center > Installed.
2. Click Advanced Media Extensions.
3. Click on Open.
4. You may need to [Sign in to your Synology account](https://github.com/007revad/Video_Station_for_DSM_722/blob/main/syno_account_sign_in.md)
5. Click on Install then OK.

<p align="center"><img src="/images/enable_hevc.png"></p>

### What about future DSM updates?

1. Update DSM.
2. Package Center will show Advanced Media Extensions as "incompatible with your DSM".
3. Run this script again.

</br>

<!--
### Screenshots

<p align="center">Description of image 1 goes here</p>
<p align="center"><img src="/images/IMAGE_NAME.png"></p>

<br>

<p align="center">Description of image 2 goes here</p>
<p align="center"><img src="/images/IMAGE_NAME.png"></p>
-->
