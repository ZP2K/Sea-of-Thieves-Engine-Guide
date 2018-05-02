# Sea of Thieves Engine Guide


#### SDK
[SoT SDK Dump](https://github.com/pubgsdk/SoT-SDK)  

#### FindPattern Signatures
```
GObjects:
89 1D ? ? ? ? 48 8B DF 48 C1 E3 04 33 D2
offset = address + 2
(GObjects)address + 6 + offset
\x89\x1D\x00\x00\x00\x00\x48\x8B\xDF\x48\xC1\xE3\x04\x33\xD2
xx????xxxxxxxxx

GNames
48 8B 3D ? ? ? ? 48 85 FF 75 ? B9 ? ? ? ? E8 ? ? ? ? 48 8B F8 48 89 44
offset = address + 3
(GNames)(*)address + 7 + offset
\x48\x8B\x3D\x00\x00\x00\x00\x48\x85\xFF\x75\x00\xB9\x00\x00\x00\x00\xE8\x00\x00\x00\x00\x48\x8B\xF8\x48\x89\x44
xxx????xxxx?x????x????xxxxxx

UWorld:
48 8B 0D ? ? ? ? 48 8B 01 FF 90 ? ? ? ? 48 8B F8 33 D2 48 8D 4E
offset = address + 3
(UWorld)(*)address + 7 + offset
\x48\x8B\x0D\x00\x00\x00\x00\x48\x8B\x01\xFF\x90\x00\x00\x00\x00\x48\x8B\xF8\x33\xD2\x48\x8D\x4E
xxx????xxxxx????xxxxxxxx
```
