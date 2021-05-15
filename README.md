# app-data-file-exec
[Magisk](https://github.com/topjohnwu/Magisk) [module](https://topjohnwu.github.io/Magisk/guides.html) allowing execution of binaries in apps `data` folder

### What does

1. Modifies one `Android` `SELinux` rule.

### Why does
1. Fixes [Elementum](https://github.com/elgatito/plugin.video.elementum) on [Kodi](https://kodi.tv/) version 19+ and `Android` version 10+
> [Elementum](https://github.com/elgatito/plugin.video.elementum) fails to start on [Kodi](https://kodi.tv/) version 19+ and `Android` version 10+ with error `Daemon error: b"PermissionError(13, 'Permission denied')"`. Issue is `Android` version 10+ [SELinux](https://source.android.com/security/selinux) [restriction](https://android.googlesource.com/platform/system/sepolicy/+/master/private/app_neverallows.te#54) for executing binaries located in application `data` folder.
> 
> Solution has been [suggested](https://github.com/elgatito/plugin.video.elementum/issues/669#issuecomment-804882665) by **@notgood**

#### How to install (exact steps for `Magisk` 23.0)

1. [Download](https://github.com/galeksandrp/app-data-file-exec/releases/latest) `.zip` asset to device
2. Open `Magisk Manager`
3. Tap `Modules` tab (first tab on the right, with `puzzle` icon)
4. Tap `Install from storage` button
5. Choose downloaded `.zip`
6. Wait for `- Done` message
7. Reboot device

#### Troubleshooting

- Q: `! Unzip error`
- A: You downloaded `Source code (zip)` instead of `.zip` asset.

#### What contains and redistributes

| File | SPDX License Identifier |
| - | - |
| `META-INF/com/google/android/update-binary` | [GPL-3.0-only](https://spdx.org/licenses/GPL-3.0-only.html) |

#### Github topics
`magisk` `magisk-module` `magisk-modules` `android` `root` `selinux` `selinux-policy`
