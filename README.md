ATH9KFixup
==========
This fork is adjusted to be loaded with [OCLP's patched El Capitan](https://github.com/dortania/OpenCore-Legacy-Patcher/tree/main/payloads/Kexts/Wifi) **AirportAtheros40.kext**

An open source kernel extension providing patches for unsupported Atheros cards.
- AR946X (AR9462 & AR9463)
- AR9485
- AR9565

#### Features
Boot args:
- AR946X: (Default)
- AR9485: -ath9485
- AR9565: -ath9565

Load kext in order:

1. ATH9Fixup.kext
2. corecaptureElCap.kext
3. IO80211ElCap.kext
4. IO80211ElCap.kext/Contents/PlugIns/AirPortAtheros40.kext

Set minKernel to `18.0.0` (Mojave)

#### Credits
- [Apple](https://www.apple.com) for macOS  
- [vit9696](https://github.com/vit9696) for [Lilu.kext](https://github.com/vit9696/Lilu) & for patch
- [Pike R. Alpha](https://github.com/Piker-Alpha) for patch
- [lvs1974](https://applelife.ru/members/lvs1974.53809/) for original source code and idea
- [chunnann](http://www.insanelymac.com/forum/user/1977171-chunnann/) for writing the software and maintaining it
- [unitedastronomer](https://github.com/unitedastronomer) adjusted to be used with OCLP's patched AirportAtheros40
