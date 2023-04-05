<p align="center">

<img src="https://github.com/litmusos/manifest/blob/thirteen/Litmus.png">

</p>

# Litmus OS #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/litmusos/manifest -b thirteen

```

```bash

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch aosp_$device-userdebug

# Build the code
$ mka bacon -jX
```
