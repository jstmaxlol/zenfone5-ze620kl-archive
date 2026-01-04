# asus zenfone 5 (2018-ish), ze620kl modding archive
### NOTE! I AM STILL UPLOADING SOME FILES.

i made this repo because asus mostly killed mirrors and literally anything for this phone \
basically i got this phone off my brother and i wanted to have fun (_aka, mod it_). 

after finding that most official mirrors to do literally ANYTHING with this brick are dead \
i went digging and found the files found in this repo, in this readme ill quickly run down \
every file i put here so you can use them for your own modding purposes.

i also want to thanks [Conobi](https://github.com/Conobi), and his repo [Conobi/asus_x00qd_files](https://github.com/Conobi/asus_x00qd_files), thanks to which i was easily able to find: 
- (un?)official TWRP 3.3.0 [(mirror from his repo)](https://github.com/Conobi/asus_x00qd_files/raw/refs/heads/master/TWRP_3.3.0_ZE620KL_190428.img) image (`twrp.img`)
- technically also the UnlockApp from asus, but the app does not work as they [killed the backend in around 2021-2022(?)]()

# files
- twrp [(download)](https://github.com/jstmaxlol/zenfone5-ze620kl-archive/raw/refs/heads/master/twrp.img)
- android 10 oem beta build [(download)](https://github.com/jstmaxlol/zenfone5-ze620kl-archive/raw/refs/heads/master/UL-ASUS_X00QD-ASUS-AOSP-17.0615.2005.25-1.1.1-user.zip), for more info on how i got this file see [this](#android-10-oem-beta-build)

## android 10 oem beta build
this android 10 beta build is very important because it's most likely the only way anyone (_after the shutdown_) \
may be able to actually mod this phone. \
i found it thanks to [this post](https://zentalk.asus.com/t5/zenfone-5-series/zenfone-5-ze620kl-unlock-bootloader-failed/td-p/109897) on the asus forums, where the user ErwinGau blessed us \
with [this](https://zentalk.asus.com/t5/zenfone-5-series/zenfone-5-ze620kl-unlock-bootloader-failed/m-p/354750#M10898) simple tutorial on how to unlock the bootloader. \
the post linked to [this _now dead_]() mirror to this magic android 10 build that you **need** to unlock the bootloader. \
as i said, the link is now dead, but thanks to the _i cant thank them enough_ aka **internet archive** i were able to \
find the download link to the original zip file, [(download)](), **note that i _highly_ recommend downloading the build from \
from this repo instead of that archive.org mirror because i (_with a 2.5 gigabit_) connection took around 6-7 (_dont say it_) \
hours to complete the download.**
also, whislt downloading with `aria2`, it crashed because it got an EOF, after that i restarted the same command to resume, \
but the mirror kept refusing and sending EOF, because of that i was going insane and i tried the other mirror from the internet \
archive, [(this one)](https://web.archive.org/web/20230721104032/https://dlcdnets.asus.com/pub/ASUS/ZenFone/ZE620KL/UL-ASUS_X00QD-ASUS-AOSP-17.0615.2005.25-1.1.1-user.zip), after resuming with this mirror it worked.
