

# How to mine Zent Cash with XMRig

<span style="color:red">**Important note**</span>: All mining software is detected by antivirus as a threat.

[TOC]

1.- Download Xmrig from GitHub

https://github.com/xmrig/xmrig

> This software has not been developed by the Zent team, so we cannot be held responsible if any problems occur when using this tool.

## **Windows / Linux:**

Is recommeded download the builded binary from Release section https://github.com/xmrig/xmrig/releases.

Scroll down and find the latest release for your SO.

![image-20210505183138911](C:\Users\csanc\OneDrive\PROYECTOS\ZENT\DOCS\Step-by-step\IMG\github-download-release)

Is possible your browser show a message like this:

![Browser Error](C:\Users\csanc\OneDrive\PROYECTOS\ZENT\DOCS\Step-by-step\IMG\download-error-en)

Click on ![Show all Button](C:\Users\csanc\AppData\Roaming\Typora\typora-user-images\image-20210505191851208.png)

![Keep dangerous file](C:\Users\csanc\AppData\Roaming\Typora\typora-user-images\image-20210505191922955.png)

![Keep Anyway](C:\Users\csanc\AppData\Roaming\Typora\typora-user-images\image-20210505191950680.png)

Uncompress the zip file.

Windows Defender or other antivirus will detect the miner like a trojan.

- Click on the Antivirus message
- Select Keep File or Restore file



## **Linux Building:**

Here are the complete instructions to build the source code: https://xmrig.com/docs/miner/build



## Start Mining

##### If you can use your GPU for mining

- #### nVidia CUDA

Download the ZIP file https://github.com/xmrig/xmrig-cuda/releases, this ZIP contains the libraries to use your GPU for mining.

> If you don´t know your CUDA version, you can find information here: https://developer.nvidia.com/cuda-gpus

- #### AMD OpenCL

Download the ZIP file https://github.com/xmrig/xmrig-amd/releases, this ZIP contains the libraries to use your GPU for mining.

**In both cases it is only necessary to extract the ZIP files in the folder where the xmrig executable is located.**

### Run this command:

**Change the address to yours**: *Ze3eeYHXfJH2SaghicPsKgdP6HC5ehZHe4uRCmi92rpTYRhS6oSeu6E4QKzodiSHTgNf9Yks743cteLQ875Pfnny2GfV2ihDq*

If you´re using GPU  to mining (Windows / Linux / Mac):

- Add `--opencl` after xmrig for AMD Graphic Cards
- Add `--cuda` after xmrig for NVIDIA Graphic Cards

Windows:

```bash
# CPU
xmrig.exe -o https://pool001.zent.cash:5555 -u Ze3eeYHXfJH2SaghicPsKgdP6HC5ehZHe4uRCmi92rpTYRhS6oSeu6E4QKzodiSHTgNf9Yks743cteLQ875Pfnny2GfV2ihDq -k -a cn-pico
```

```bash
# AMD
xmrig.exe --opencl-o https://pool001.zent.cash:5555 -u Ze3eeYHXfJH2SaghicPsKgdP6HC5ehZHe4uRCmi92rpTYRhS6oSeu6E4QKzodiSHTgNf9Yks743cteLQ875Pfnny2GfV2ihDq -k -a cn-pico
```

```bash
# NVIDIA
xmrig.exe --cuda -o https://pool001.zent.cash:5555 -u Ze3eeYHXfJH2SaghicPsKgdP6HC5ehZHe4uRCmi92rpTYRhS6oSeu6E4QKzodiSHTgNf9Yks743cteLQ875Pfnny2GfV2ihDq -k -a cn-pico
```

Linux:

```bash
./xmrig -o https://pool001.zent.cash:5555 -u Ze3eeYHXfJH2SaghicPsKgdP6HC5ehZHe4uRCmi92rpTYRhS6oSeu6E4QKzodiSHTgNf9Yks743cteLQ875Pfnny2GfV2ihDq -k -a cn-pico
```

Mac:

```bash
./xmrig -o https://pool001.zent.cash:5555 -u Ze3eeYHXfJH2SaghicPsKgdP6HC5ehZHe4uRCmi92rpTYRhS6oSeu6E4QKzodiSHTgNf9Yks743cteLQ875Pfnny2GfV2ihDq -k -a cn-pico
```

Happy mining!!!