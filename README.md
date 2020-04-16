# Only the vulkan part of AMDGPU-PRO drivers

Can live next to RADV

 https://www.amd.com/en/support/kb/release-notes/rn-amdgpu-unified-linux

Start your game/app with either:
- `VK_ICD_FILENAMES=/opt/amdgpu-pro/etc/vulkan/icd.d/amd_icd64.json` for 64-bit
or
- `VK_ICD_FILENAMES=/opt/amdgpu-pro/etc/vulkan/icd.d/amd_icd32.json` for 32-bit


You can also pass `VK_ICD_FILENAMES=/opt/amdgpu-pro/etc/vulkan/icd.d/amd_icd64.json:/opt/amdgpu-pro/etc/vulkan/icd.d/amd_icd32.json` if unsure.


## Build:
```
git clone https://github.com/Frogging-Family/amdgpu-pro-vulkan-only.git
cd amdgpu-pro-vulkan-only
makepkg -si
```
