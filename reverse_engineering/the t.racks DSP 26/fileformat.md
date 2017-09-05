# the t.racks DSP 26
## Fileformat for preset-channel description
### {file}.ch6

extracted from text.ch6

`
00 00 B4 00 00 00 00 C8 13 0C 00 96 62 00 0A 05 96 0A 05 00 00 40 1C 18 00 00 58 1C 18 00 00 70 1C 18 00 00 88 1C 18 00 00 A0 1C 18 00 00 B8 1C 18 00 00 D0 1C 18 00 00 00 14 00 00 F0 00 39 00 74 65 73 74 20 20 20 20 20 20 20 20 20 20 20 20
`

?

    00 00 B4 00 00 00 00 C8 13 0C 00 96 62 00 0A 05 96 0A 05

EQ-Channel 1-7

    00: type
        00: Bell / Peaking
        01: Hi-Shelving
        02: Lo-Shelving
    00: ?
    40: frequency
        00 (20Hz) - F0 (20.000Hz)
    1C: value
        00 - 64
    18: value (dB)
        00 (-12dB) - 30 (12dB)
    ---
    00 00 58 1C 18  EQ2
    00 00 70 1C 18  EQ3
    00 00 88 1C 18  EQ4
    00 00 A0 1C 18  EQ5
    00 00 B8 1C 18  EQ6
    00 00 D0 1C 18  EQ7

?

    00: ?
    00: EQ enable/disable
        Bitmask
        Bit 1-7 = EQ 1-7
    00: ?
    00: frequency High Pass Filter
        00 (20Hz) - F0 (20.000Hz)
    00: slope High Pass Filter
    00: ?
    F0: frequency Low Pass Filter
        00 (20Hz) - F0 (20.000Hz)
    00: slope Low Pass Filter
    39: Bitmask Bypass (EQ / Limiter / DLF)
    00: ?

Footer

    74 65 73 74 20 20 20 20 20 20 20 20 20 20 20 20
    Name of the file, always 16 Bytes
    truncated if longer
    filled with space if shorter
