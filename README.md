All code is written in C

For file DDT of IVLBC; simply running it without any modifications is sufficient.

For file Key_Schedule_IVLBC-80 and Key_Schedule_IVLBC-128; to determine which round‑key bits in RKj can be derived from known bit values in RKi, enter the bit positions you know (0–63) into the “tracked” section, and set the “rounds” section to j−i. Known key bits are marked with an asterisk (*).

For file Mixcolumn Operation of IVLBC; simply running it without any modifications is sufficient.

For file differential_trail_prob_sum_of_IVLBC; In the main function, mark each known input‐active nibble by setting "in.active[i] = 1" (where i is its index) and each known output‐active nibble by setting "tgt.active[j] = 1" (where j is its index), then set "total_rounds = n" (the number of rounds) and simply compile and run the program to compute the total probability of all MixColumn operations for the given characteristic.
