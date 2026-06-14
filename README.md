# Kernel — Xiaomi Redmi 4X (santoni) MSM8937

Kernel source for keepQASSA Sisu (Android 10) on Xiaomi Redmi 4X (santoni).

## Specs

| Spec | Detail |
|------|--------|
| Kernel | 4.9.267 |
| SoC | Qualcomm MSM8937 (Snapdragon 435) |
| Arch | ARM64 |
| Defconfig | `santoni_defconfig` |
| CPU Cluster 0 | big (cpu0-3): 960–1497 MHz |
| CPU Cluster 1 | little (cpu4-7): 768–1209 MHz |
| GPU | Adreno 505: 19.2–450 MHz |

## Build

```bash
# In ROM source tree
source build/envsetup.sh
lunch qassa_santoni-userdebug
mka qassa -j10
```

Kernel is built inline with the ROM — no separate kernel build needed.

## Defconfigs

| Config | Description |
|--------|-------------|
| `santoni_defconfig` | Main defconfig for qassa build |
| `santoni-stock_defconfig` | Stock kernel config |
| `santoni_treble_defconfig` | Treble-enabled config |

## Related Repos

| Repo | Branch | Description |
|------|--------|-------------|
| [device_xiaomi_santoni_qassa](https://github.com/ziachi/device_xiaomi_santoni_qassa/tree/qassa-dev) | `qassa-dev` | Device tree |
| [vendor_xiaomi_santoni_qassa](https://github.com/ziachi/vendor_xiaomi_santoni_qassa/tree/10.0) | `10.0` | Vendor blobs |

## Maintainer

**[@kalomakan](https://t.me/kalomakan) / [ziachi](https://github.com/ziachi)**
