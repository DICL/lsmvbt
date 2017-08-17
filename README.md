# LS-MVBT
In this work, we developed multi-version B-tree with lazy split (LS-MVBT) to resolve the journaling of journal anomaly in Android I/O. The contribution of LS-MVBT consists of two key elements:(i) **Multi-version B-tree**  effectively reduces the number of fsync() calls. (ii) it significantly reduces "the number of dirty pages to be synchronized in a single fsync() call" via optimizing multi-version B-tree for Android I/O. The optimization consists of five elements: **Lazy split**, **Buffer reservation**, **Metadata embedding"", ""Lazy garbage collection**, and **Disabling sibling redistribution**. 

## Reference:

Wook-Hee Kim, Beomseok Nam, Dongil Park, and Youjip Won 
"Resolving Journaling of Journal Anomaly in Android I/O: Multi-Version B-tree with Lazy Split", 
12th USENIX Conference on File and Storage Technologies (USENIX FAST '14), Santa Clara, CA, Feb. 2014.

https://www.usenix.org/system/files/conference/fast14/fast14-paper_kim-wook-hee.pdf

## Acknowledgement:

This research was supported by MKE/KEIT (No.10041608, Embedded System Software for New Memory based Smart Devices).
