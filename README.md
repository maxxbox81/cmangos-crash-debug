# cmangos-crash-debug

Collection of patch files to prevent known crashes and memory errors in the CMaNGOS core.
➡️ Also see the [CMaNGOS module crash patch collection](https://github.com/maxxbox81/cmangos-crash-module-debug)

## 🛠️ Included Patches

| Patch File | Description | Crash Screenshot |
|------------|-------------|------------------|
| [0001-fix-ObjectGridLoader-LoadHelper-crash.patch](0001-fix-ObjectGridLoader-LoadHelper-crash.patch) | Fixes a potential crash in `LoadHelper` caused by `IsInWorld()` assertion failure | [1️⃣ View](images/Objektgridloadererror_0001_1.png)<br>[2️⃣ View](images/Objektgridloadererror_0001_2.png) |

## 💡 Usage

```bash
cd /opt/cmangos/mangos
git apply /opt/cmangos/mangos/patches/0001-fix-ObjectGridLoader-LoadHelper-crash.patch
