# HungNT 3rd-party: Hot Reload

Asset gốc: [Hot Reload — Edit Code Without Compiling (The Naughty Cult)](https://assetstore.unity.com/packages/tools/utilities/hot-reload-edit-code-without-compiling-254358)

## Cài đặt

> Lưu ý: package id vẫn là `com.singularitygroup.hotreload` (KHÔNG đổi), nên **key** trong manifest phải là id đó, còn URL trỏ tới repo `com.hungnt.thirdparty.hotreload`.

Thêm vào `Packages/manifest.json`:

```json
"com.singularitygroup.hotreload": "https://github.com/HungNT-UPM/com.hungnt.thirdparty.hotreload.git"
```

Hoặc Package Manager → **Add package from git URL...**:

```
https://github.com/HungNT-UPM/com.hungnt.thirdparty.hotreload.git
```

## Note

- Đây là package Hot Reload chính thức được wrap lại (GitHub-only), giữ nguyên toàn bộ namespace/asmdef gốc `SingularityGroup.HotReload`.
- Package có ship **native binaries** (DLL `RuntimeDependencies`, `HotReloadNativeHelper.dylib`...).
- Package id cố ý để nguyên `com.singularitygroup.hotreload` — asset hardcode đường dẫn theo tên này, đổi id sẽ làm hỏng package.
