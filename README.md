# Grid Autosport Mobile Graphics Optimizer for Android

[![Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://android.com)
[![No Root](https://img.shields.io/badge/Root-Not%20Required-blue.svg)](https://github.com)
[![Tested](https://img.shields.io/badge/Tested-Pixel%207a-orange.svg)](https://github.com)

Simple guide to modify [Grid Autosport](https://play.google.com/store/apps/details?id=com.feralinteractive.gridas&hl=en_IN) graphics settings on Android devices without root access.

## 📱 Requirements

- Android phone with Grid Autosport installed
- Computer (Windows/Mac/Linux)
- [LocalSend](https://localsend.org/) or USB cable for file transfer
- Text editor (VSCode, Notepad++, etc.)

## 🚀 Step-by-Step Guide

### Step 1: Get the Preferences File

Navigate to this folder on your Android device:

```
android/data/com.feralinteractive.gridas/files/feral_app_support/preferences
```

### Step 2: Transfer to Computer

Use [LocalSend](https://localsend.org/) or USB cable to copy the `preferences` file to your computer.

### Step 3: Edit Graphics Settings

Open the file in any text editor and search for these settings:

```xml
<!-- Game Version (Check before replacing) -->
<value name="GameVersionString" type="string">GRID™ Autosport v1.10.5</value>

<!-- Screen Resolution Settings -->
<value name="FixedScreenHeight" type="integer">720</value>
<value name="ScreenH" type="integer">720</value>
<value name="ScreenW" type="integer">1280</value>

<!-- FPS Settings -->
<value name="gfxconfig_max_fps" type="integer">60</value>
<value name="gfxconfig_high_max_fps" type="integer">60</value>

<!-- Performance Settings (Keep OFF for better performance) -->
<value name="gfxconfig_advanced_lighting" type="string">off</value>
<value name="gfxconfig_high_advanced_lighting" type="string">off</value>
<value name="gfxconfig_multisampling" type="string">off</value>
<value name="gfxconfig_high_multisampling" type="string">off</value>
<value name="gfxconfig_default_multisampling" type="string">off</value>

<!-- Visual Quality Settings (Options: low, medium, high, ultrahigh) -->
<value name="gfxconfig_advanced_fog" type="string">on</value>
<value name="gfxconfig_anisotropic_filtering" type="string">ultrahigh</value>
<value name="gfxconfig_car_reflection" type="string">high</value>
<value name="gfxconfig_cloth" type="string">high</value>
<value name="gfxconfig_crowd" type="string">high</value>
<value name="gfxconfig_default_preset_name" type="string">high</value>
<value name="gfxconfig_dynamic_ambient_occ" type="string">high</value>
<value name="gfxconfig_dynamic_ambient_occ_soft" type="string">on</value>
<value name="gfxconfig_global_illumination" type="string">on</value>
<value name="gfxconfig_groundCover" type="string">on</value>
<value name="gfxconfig_mirrors" type="string">high</value>
<value name="gfxconfig_night_lighting" type="string">high</value>
<value name="gfxconfig_objects" type="string">high</value>
<value name="gfxconfig_particles" type="string">high</value>
<value name="gfxconfig_preset_name" type="string">custom</value>
<value name="gfxconfig_shaders" type="string">high</value>
<value name="gfxconfig_shadows" type="string">high</value>
<value name="gfxconfig_skidmarks" type="string">on</value>
<value name="gfxconfig_textures" type="string">high</value>
<value name="gfxconfig_track" type="string">high</value>
<value name="gfxconfig_trees" type="string">high</value>
<value name="gfxconfig_vehicles" type="string">high</value>
<value name="gfxconfig_voice_count" type="string">high</value>
<value name="gfxconfig_water" type="string">high</value>

<!-- High Preset Settings -->
<value name="gfxconfig_high_advanced_fog" type="string">on</value>
<value name="gfxconfig_high_anisotropic_filtering" type="string">ultrahigh</value>
<value name="gfxconfig_high_car_reflection" type="string">high</value>
<value name="gfxconfig_high_cloth" type="string">high</value>
<value name="gfxconfig_high_crowd" type="string">high</value>
<value name="gfxconfig_high_dynamic_ambient_occ" type="string">high</value>
<value name="gfxconfig_high_dynamic_ambient_occ_soft" type="string">on</value>
<value name="gfxconfig_high_global_illumination" type="string">on</value>
<value name="gfxconfig_high_groundCover" type="string">on</value>
<value name="gfxconfig_high_mirrors" type="string">high</value>
<value name="gfxconfig_high_night_lighting" type="string">high</value>
<value name="gfxconfig_high_objects" type="string">high</value>
<value name="gfxconfig_high_particles" type="string">high</value>
<value name="gfxconfig_high_shaders" type="string">high</value>
<value name="gfxconfig_high_shadows" type="string">high</value>
<value name="gfxconfig_high_skidmarks" type="string">on</value>
<value name="gfxconfig_high_textures" type="string">high</value>
<value name="gfxconfig_high_track" type="string">high</value>
<value name="gfxconfig_high_trees" type="string">high</value>
<value name="gfxconfig_high_vehicles" type="string">high</value>
<value name="gfxconfig_high_voice_count" type="string">high</value>
<value name="gfxconfig_high_water" type="string">high</value>
```


### Step 4: Transfer Back

1. Save the edited file
2. Transfer back to your phone using LocalSend or USB
3. Replace the original file in the same location
4. Launch Grid Autosport

## 📂 Ready-Made Preference File

I'll share my optimized preference file in this repo. **Important:** Check your game version before using:

```xml
<value name="GameVersionString" type="string">GRID™ Autosport v1.10.5</value>
```


If your version is different, edit the settings manually instead of replacing the entire file.

## 🎯 Device Recommendations

**High-End Devices:** Use all settings as shown above  
**Mid-Range (Pixel 7a):** Use 720p settings as provided  
**Budget Devices:** Change quality settings to `medium` or `low`, set FPS to `30`

## ❓ Quick FAQ

**Q: Is this safe?**  
✅ Yes, you're only editing configuration files.

**Q: Will game updates reset settings?**  
⚠️ Yes, keep your edited file as backup.

**Q: Game won't start after changes?**  
🔧 Restore the original preferences file.

---

**Tested on Google Pixel 7a (8GB/128GB) - Works perfectly!**

*If this helped you, please ⭐ star this repo!*
