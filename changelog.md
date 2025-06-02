## Changelogs

**v1.1 - 20250601**

1. Basically fixed control center animation drop/slow motion issues on A15 HyperOS 2.
2. Updated EEVDF patchset to Linux mainline and further complement upstream scheduler backports to improve smoothness and power consumption.
3. Updated PSI to improve its performance and fix some issues, which indirectly improves lmkd's memory reclaiming strategy.
4. Corrected CPU cluster topology to improve scheduling decisions using DynamIQ Shared Unit.
5. Updated lz4 to v1.10.0 and zstd to v1.5.7.
6. Removed MGLRU to solve possible OOM issues under high memory pressure.
7. Removed unused reap_mem_on_sigkill feature to prevent userspace from enabling it.
8. Set swappiness to 60% (Linux default) to improve smoothness under high memory pressure.
9. Reduced vmstat interval from 20 seconds to 10 seconds to help lmkd make better decisions.
10. Replaced per-process reclaim with process_madvise from upstream.
11. Switched the default sleep mode from s2idle back to deep sleep, and disabled s2idle that may cause problems.
12. Compiled the kernel with ThinLTO and added more compilation optimization flags.
13. Updated KernelSU version to v1.0.5-2-legacy.
14. And more optimizations, adjustments and fixes.

**20250227 version**

1. Renamed kernel name from Rikka to Zundamon.
2. Switched KernelSU variant to https://github.com/rsuntk/KernelSU.
3. Upstreamed EEVDF to Linux-mainline state, significantly improved smoothness and power consumption.
4. Further complemented upstream scheduler backports, improved idle core selection etc.
5. Updated CASS to make it work better with UClamp, thus improved power consumption.
6. Updated Binder driver from upstream, improved descriptor lookup speed.
7. Updated Jump label and LSE atomics from upstream, improved the performance of some scenes.
8. Dropped manually set power-efficient workqueues.
9. And more misc optimizations and fixes.
