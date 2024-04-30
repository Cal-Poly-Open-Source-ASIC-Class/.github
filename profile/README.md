# Computer Architecture Research Project (CARP)
Welcome to the home of Cal Poly's CARP, an ongoing group/club dedicated to open source chip design. 

# Getting Started



## Tools
All of these tools work best on Linux. 
- If you are on Windows, install [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install). Complete the following installations from within WSL. Also see using [WSL with VSCode](https://code.visualstudio.com/docs/remote/wsl).
- If you are on Mac, you can install tools natively, with varying support.

### OSS Cad Suite
OSS Cad Suite bundles all of the necessary open source tools for digital design, inclduing:
- __Verilator__ for Linting & Simulation
- __CocoTB__ for Testing
- __Yosys__ for Synthesis
- __GTKWave__ for viewing waveforms

To install, follow the instructions here: 
https://github.com/YosysHQ/oss-cad-suite-build

In summary,
1. Download the archive depending on your system here: 
https://github.com/YosysHQ/oss-cad-suite-build/releases/latest
2. Extract it to somewhere accessible, such as your home directory `~`
3. Run the following command in EVERY terminal that needs OSS Cad Suite Tools:
`source <extracted_location>/oss-cad-suite/environment`

### RISC-V Toolchain
The RISC-V toolchain lets us compile C and Assembly files to get RISC-V machine code, as well as debug that code. 

To install on Linux or WSL, follow the instructions here:
https://github.com/stnolting/riscv-gcc-prebuilt


Example Installation on Linux:
```
wget https://github.com/stnolting/riscv-gcc-prebuilt/releases/download/rv32i-131023/riscv32-unknown-elf.gcc-13.2.0.tar.gz
sudo mkdir /opt/riscv
sudo tar -xzf riscv32-unknown-elf.gcc-13.2.0.tar.gz -C /opt/riscv/
echo "export PATH=$PATH:/opt/riscv/bin" >> ~/.bashrc
```

To install on Mac, follow these instructions:
https://github.com/riscv-software-src/homebrew-riscv