🌸✨ uchan (ucan) Clang OS Toolchain ✨🌸

⚠️ Please read this first
Hi~ welcome to the uchan (ucan) clang OS toolchain!
This is not just any clang—it’s a custom version made with love 💖 for kernel builders, ROM tweakers, or anyone who loves coding with a lil’ wibu spice 🐰💻

📖 Description

Custom LLVM/Clang toolchain by uchan (ucan) 🌸

Vendor: uchan (ucan) clang OS

Compiler: clang, clang++

Linker: ld.lld

Optimizer: Polly Loop Optimizer ✨

Sanitizers: compiler-rt 🛡️

Targets: x86_64, AArch64, ARM, RISCV, BPF 🐾

Build Type: Stage1-only for stability ⚡

Optimized for kernel & system-level builds. Perfect for:
✔️ Kernel building
✔️ ROM tweaks
✔️ Wibu-style compilation 🐱‍👤💖

⚙️ Installation
# Extract toolchain
tar -xf uchan-clang-os-toolchain.tar.xz -C /opt/

# Add to PATH
export PATH="/opt/uchan-clang/bin:$PATH"

# Check clang vendor string
clang -v   # Vendor: uchan (ucan) clang OS

💡 Usage Examples
🔹 Compile a simple program
echo 'int main() { return 0; }' > test.c
clang test.c -o test
./test
echo $?   # Should output 0 😎

🔹 Build Linux Kernel
git clone https://github.com/torvalds/linux.git
cd linux

make LLVM=1 LLVM_IAS=1 CC=clang LD=ld.lld defconfig
make LLVM=1 LLVM_IAS=1 CC=clang LD=ld.lld -j$(nproc)


Your kernel will compile successfully with a wibu smile 😸💖

📂 Installed Files

/opt/uchan-clang/bin/ → clang, clang++, ld.lld, llvm-*

/opt/uchan-clang/lib/ → libraries, compiler-rt

/opt/uchan-clang/include/ → headers

📝 Release Notes

✨ Custom vendor string: uchan (ucan) clang OS
✨ Stable stage1-only build
✨ LLD linker included
✨ Polly optimizer enabled
✨ Compiler-rt sanitizers
✨ Multi-arch target ✅
✨ Test compile & kernel build = PASSED 😻

⚠️ Known Issues

Extracting to /opt/ may require root access 🐾

If ninja install errors occur, use manual install or DESTDIR workaround

## 🌸 Support / Donations 🌸

Konbanwa~ 💕  
If you like this toolchain and want to support its development (so I can buy more 🍵 tea & 🐾 neko snacks while coding 😆), you can donate via:

<a href="https://www.buymeacoffee.com/ucann" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/H2H61M46VE)

[![Support on Trakteer](https://img.shields.io/badge/☕_Support-Trakteer-red?style=for-the-badge)](https://trakteer.id/ucann)

[![Donate on Saweria](https://i.ibb.co.com/xctGvQY/download.png) ](https://saweria.co/ucan01)

Every support makes the creator’s heart melt 🥹💖
Thank you so much~ 😘🌸

Wibu Words & Motivation:

Keep coding with warm tea 🍵💖

Don’t forget to rest 😽✨

Compiling is like cooking ramen: patience + love 🍜💖

Errors aren’t sad—they’re just the compiler smiling 😹💞

May your projects run smoothly, your heart be happy, and RAM stay fast 🐰💻💖

Have Fun & Keep Wibu Coding! 🌸
