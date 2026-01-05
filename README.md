# asus zenfone 5 (2018-ish), ze620kl modding archive
> project status: **temporarily halted, looking for a solution to unlock the bootloader**

i made this repo because asus mostly killed mirrors and literally anything for this phone \
basically i got this phone off my brother and i wanted to have fun (_aka, mod it_). 

after finding that most official mirrors to do literally ANYTHING with this brick are dead \
i went digging and found the files collected in this repo, in this readme ill quickly run down \
every file i put here so you can use them for your own modding purposes.

i also want to thank [Conobi](https://github.com/Conobi), and their repo [Conobi/asus_x00qd_files](https://github.com/Conobi/asus_x00qd_files), thanks to which i was easily able to find: 
- (un?)official TWRP 3.3.0 [(mirror from his repo)](https://github.com/Conobi/asus_x00qd_files/raw/refs/heads/master/TWRP_3.3.0_ZE620KL_190428.img) image (`twrp.img`)
- technically also the [UnlockApp](https://github.com/Conobi/asus_x00qd_files/raw/refs/heads/master/UnlockApp_ZE620KL_9_1_0_1_180130.apk) from asus, but the app does not work as they [killed the backend in](https://zentalk.asus.com/t5/zenfone-5-series/zenfone-5-ze620kl-unlock-bootloader-failed/m-p/109899/highlight/true#M4873) [around 2023-ish](https://www.reddit.com/r/Android/comments/15isa1l/asus_is_taking_back_the_ability_to_unlock_the/).

# files
- twrp [(download)](https://github.com/jstmaxlol/zenfone5-ze620kl-archive/raw/refs/heads/master/twrp.img)
- android 10 oem beta build [(download)](https://github.com/jstmaxlol/zenfone5-ze620kl-archive/releases/download/a10-beta-build-recvrd/UL-ASUS_X00QD-ASUS-AOSP-17.0615.2005.25-1.1.1-user.zip), for more info on how i got this file see [this](#android-10-oem-beta-build)
<!--- the `decompressed_build/` directory is the entirety of the [android 10 oem beta build](#android-10-oem-beta-build) unzipped.-->

## android 10 oem beta build
> this is **not** the stable android 10 release, but an early OEM beta build randomly linked in the zentalk forums.

&nbsp;&nbsp;&nbsp;&nbsp; this android 10 beta build is very important because it's most likely the only way anyone (_after the shutdown_) \
may be able to actually mod this phone. \
&nbsp;&nbsp;&nbsp;&nbsp; i found it thanks to [this post](https://zentalk.asus.com/t5/zenfone-5-series/zenfone-5-ze620kl-unlock-bootloader-failed/td-p/109897) on the asus forums, where the user ErwinGau blessed us \
with [this](https://zentalk.asus.com/t5/zenfone-5-series/zenfone-5-ze620kl-unlock-bootloader-failed/m-p/354750#M10898) simple tutorial on how to unlock the bootloader. \
the post linked to [this mirror](https://dlcdnets.asus.com/pub/ASUS/ZenFone/ZE620KL/UL-ASUS_X00QD-ASUS-AOSP-17.0615.2005.25-1.1.1-user.zip?model=zenfone%205%20%EF%BC%88ze620kl%EF%BC%89), **now dead**, to this magic android 10 build that you **need** to unlock the bootloader. \
&nbsp;&nbsp;&nbsp;&nbsp; as i said, the link is now dead, but thanks to the _i cant thank them enough_ aka **internet archive** i was able to \
find the download link to the original zip file, [(download)](https://web.archive.org/web/20200906162331if_/https://dlcdnets.asus.com/pub/ASUS/ZenFone/ZE620KL/UL-ASUS_X00QD-ASUS-AOSP-17.0615.2005.25-1.1.1-user.zip), **note that i _highly_ recommend downloading the build \
from this repo instead of that archive.org mirror because i (_with a 2.5 gigabit_) connection took around 6-7 (_dont say it_) hours to complete the download.** \
&nbsp;&nbsp;&nbsp;&nbsp; also, whilst downloading with `aria2`, it crashed because it got an EOF, after that i simply re-ran the same command to resume, \
but the mirror kept refusing and sending EOF, because of that i was going insane and i tried the other mirror from the internet \
archive, [(this one)](https://web.archive.org/web/20230721104032/https://dlcdnets.asus.com/pub/ASUS/ZenFone/ZE620KL/UL-ASUS_X00QD-ASUS-AOSP-17.0615.2005.25-1.1.1-user.zip), after resuming with this mirror it worked.

## download decompressed build
```bash
git lfs install
git clone https://github.com/jstmaxlol/zenfone5-ze620kl-archive.git
cd zenfone5-ze620kl-archive
git lfs pull
```

## archival note
- no warranty is provided, the given files are not mine, i just found them and linked them here.
- these files are preserved for educational and device recovery purposes.
- all trademarks and copyrights belong to ASUS.
- files are provided unmodified.

#### legal note
> The `LICENSE` file found in this repo applies only to this README (`README.md`), the repository layout, and any original scripts and/or documents.
Anything else is owned by each respective owner, ASUS owns the binary for the UnlockApp (not technically present here, but i linked it) \
Google, as part of Open Handset Alliance with its members, the Android Open Source Project and ASUS (build-specific modifications) collectively own the Android 10 OEM beta build I archived in this repo, originally hosted on the [asus.com](https://asus.com/) website.

