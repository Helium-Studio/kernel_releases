## Changelogs

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
