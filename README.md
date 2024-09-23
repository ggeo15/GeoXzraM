# geoXzram
Here are some positive and negative points of having virtual ram (zram) with the lz4 compression algorithm:

# Positives:

Better Performance: lz4 is fast in compression and decompression, resulting in lower latency and more efficient CPU usage.

Memory Saving: Allows you to store more data in compressed RAM, reducing the need for disk swaps.

Battery Life: Fewer read/write operations on storage and lower CPU consumption help save battery life.

Improved User Experience: Suitable for Devices with Less RAM: Improves performance on low and mid-range devices by effectively increasing available memory.

# Negatives:

Lower Compression: lz4 offers a lower compression ratio compared to other algorithms like lzma, resulting in less space saved in memory.

CPU Consumption: Although lz4 is efficient, compression and decompression still consume CPU resources, which can affect the performance of other processes on devices with less powerful CPUs.

Compatibility: Not all ROMs or kernels easily support changing the compression algorithm, which may limit the applicability of the solution.

Variable Impact: Positive impact may vary depending on the specific use of the device. In some cases, the benefits may be less noticeable.

# How will I know if the module is working?

use this command in your terminal emulator: su -c "cat /sys/block/zram0/comp_algorithm"

if the compression algorithm is changed by the module it should look like this: [lz4]

# Fork

add detection to see if your device is compatible with this compression algorithm
