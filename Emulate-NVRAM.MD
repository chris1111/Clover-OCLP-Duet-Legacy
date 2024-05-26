# Emulate NVRAM Clover for Ventura 13, Sonoma 14
After Post Install -> Install NVRAM (Emulate NVRAM) ⇩

🚫  Do not enable `LastBootedVolume` in the config.plist because you will get a reboot error with Startup Disk Utility!

[![Modular Image Creation](https://github.com/chris1111/Clover-OCLP-Duet-Legacy/assets/6248794/55d38a2f-1f49-4fe3-a650-76cc0114e3e1)](https://youtu.be/Mx7U41DRcDo)

* After using the command, if you change anything in the config.plist that is related to NVRAM; restart this command the same way demonstrated in the video.


# Emulate NVRAM Clover for Big Sur 11 and bellow ⇩
## View Spoiler: ⬇︎

<details> 
  <summary>NVRAM Clover for Big Sur 11 and bellow</summary>
Enable DefaultVolume=LastBootedVolume  in config.plist


![Screenshot 2024-05-26 at 6 37 34 PM](https://github.com/chris1111/Clover-OCLP-Duet-Legacy/assets/6248794/8cfcf065-ba29-4a35-96b7-6ea0bb83653e)

### Reboot macOS
* Open Terminal : type

nvram -x -p > ~/nvram.plist

![Screen Shot 2024-05-26 at 6 51 47 PM](https://github.com/chris1111/Clover-OCLP-Duet-Legacy/assets/6248794/26fa6912-3b96-4bdc-a24e-391953ae3223)


### Mount the EFI Partition
Copy and paste nvram.plist to EFI Partition

![Screen Shot 2024-05-26 at 6 52 22 PM](https://github.com/chris1111/Clover-OCLP-Duet-Legacy/assets/6248794/72c2c55b-b680-4f83-ad6a-a17978c36dc7)


### Disabled DefaultVolume=LastBootedVolume in config.plist

![Screenshot 2024-05-26 at 6 57 04 PM](https://github.com/chris1111/Clover-OCLP-Duet-Legacy/assets/6248794/ba60855e-0f21-4ec0-8b59-6e1397146e5f)

## Your get to go, reboot macOS
</details>
