# Welcome to Linux on EDU-FPGA!

## Dependencies

* fpga-icestorm
* nextpnr-ice40

```bash
# common apt dependencies
sudo apt install -y fpga-icestorm nextpnr-ice40

# toolchain to cross-compile riscv
mkdir -p ~/.local && cd ~/.local && \
wget https://github.com/xpack-dev-tools/riscv-none-elf-gcc-xpack/releases/download/v12.2.0-3/xpack-riscv-none-elf-gcc-12.2.0-3-linux-x64.tar.gz && \
tar xvf xpack-riscv-none-elf-gcc-12.2.0-3-linux-x64.tar.gz && \
chmod -R -w xpack-riscv-none-elf-gcc-12.2.0-3 && \
echo export PATH="~/.local/xpack-riscv-none-elf-gcc-12.2.0-3/bin:\${PATH}" >> ~/.bashrc && \
rm -rf xpack-riscv-none-elf-gcc-12.2.0-3-linux-x64.tar.gz 
```

## Resources

* [iCE40linux github repository](https://github.com/smunaut/iCE40linux)

