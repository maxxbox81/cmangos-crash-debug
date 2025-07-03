# cmangos-crash-debug

Collection of patch files to prevent known crashes and memory errors in the CMaNGOS core.
➡️ Also see the [CMaNGOS module crash patch collection](https://github.com/maxxbox81/cmangos-crash-module-debug)

## 🛠️ Included Patches

| Patch File | Description | Crash Screenshot |
|------------|-------------|------------------|
| [0001-fix-ObjectGridLoader-LoadHelper-crash.patch](0001-fix-ObjectGridLoader-LoadHelper-crash.patch) | Fixes a potential crash in `LoadHelper` caused by `IsInWorld()` assertion failure | [1️⃣ View](images/001_1_Objektgridloadererror.png)<br>[2️⃣ View](images/001_2_Objektgridloadererror.png) |
| [0002-cxx20-warning-suppress.patch](0002-cxx20-warning-suppress.patch) | Suppress known C++20 warnings (enum conversions, this-capture, volatile) | [1️⃣ View](images/0002_cxx20-warning-supress.png)<br> |

## 💡 Usage

```bash
cd /opt/cmangos/mangos
git apply /opt/cmangos/mangos/patches/0001-fix-ObjectGridLoader-LoadHelper-crash.patch
