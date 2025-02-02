# Overview
These steps should be performed when experiencing performance issues or after **any** DCS update.

This assumes your DCS folders are called `DCS`. If they are named differently, you will need to update the commands yourself. For example, older installs may have: `DCS.openBeta` instead of `DCS`.
# Clear Out DCS Shaders
Run the following to clear out your shaders.
## Command Prompt
```bash
rmdir /S /Q "%HOMEDRIVE%%HOMEPATH%\Saved Games\DCS\fxo"
rmdir /S /Q "%HOMEDRIVE%%HOMEPATH%\Saved Games\DCS\metashaders2"
rmdir /S /Q "%HOMEDRIVE%%HOMEPATH%\AppData\Local\DCS\"
```

---

# Clear NVIDIA Shader Cache
1. In the NVIDIA App go to `Graphics > Global Settings > Shader Cache Size` and set the value to `Disabled`.
2. **Restart** your PC. (Not shutdown!)
3. Open `Run` (Press `Windows + R`) and enter `%localappdata%low`. Click `OK`.
4. Open `NVIDIA > PerDriverVersionFolder > DXCache`.
5. Delete everything in this folder.
6. In the NVIDIA App go to `Graphics > Global Settings > Shader Cache Size` and set the value to `Unlimited`.
7. **Restart** your PC. (Not shutdown!)