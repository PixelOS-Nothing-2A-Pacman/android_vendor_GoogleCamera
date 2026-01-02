android_vendor_GoogleCamera
===================
## How to use

1. Clone the repository to `vendor/GoogleCamera`

2. Extract the APK (required due to file size limits):
   **Linux:**
   ```bash
    cd vendor/GoogleCamera/prebuilt
    7z x xxx.7z.001
   ```

3. Add this line to your `device.mk` file in your device tree:
   ```make
   $(call inherit-product-if-exists, vendor/GoogleCamera/config.mk)
   ```