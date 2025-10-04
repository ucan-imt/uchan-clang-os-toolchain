🌸✨ uchan (ucan) clang OS Toolchain ✨🌸

⚠️ Please read this first~
Hi~ Welcome to the uchan (ucan) clang OS toolchain!
This is not just any clang—it’s a custom version made with love 💖, for those who enjoy coding, kernel building, or just want to try something wibu yet serious~ 🐰💻

Description:
Custom LLVM/Clang toolchain by uchan (ucan) 🌸

Vendor: uchan (ucan) clang OS

Compiler: clang + clang++

Linker: ld.lld

Optimizer: Polly Loop Optimizer

Sanitizers: Compiler-rt

Multi-arch target: x86_64, AArch64, ARM, RISCV, BPF 🐾

Stage1-only build for stability ⚡

Optimized for kernel & system-level builds

Perfect for kernel building, ROM tweaks, or just wibu-style compilation 🐱‍👤💖

Installation:

Extract the toolchain:
tar -xf uchan-clang-os-toolchain.tar.xz -C /opt/

Add to PATH:
export PATH="/opt/uchan-clang/bin:$PATH"

Check clang version:
clang -v
(Vendor: uchan (ucan) clang OS)

Usage Examples:

Compile a simple program:
echo 'int main() { return 0; }' > test.c
clang test.c -o test
./test
echo $? # Should output 0 😎

Build Linux Kernel:
git clone https://github.com/torvalds/linux.git

cd linux
make LLVM=1 LLVM_IAS=1 CC=clang LD=ld.lld defconfig
make LLVM=1 LLVM_IAS=1 CC=clang LD=ld.lld -j$(nproc)

Your kernel compiles successfully with a wibu smile 😸💖

Files Installed:

/opt/uchan-clang/bin/ → clang, clang++, ld.lld, llvm-*

/opt/uchan-clang/lib/ → libraries, compiler-rt

/opt/uchan-clang/include/ → headers

Release Notes:

Custom vendor string: uchan (ucan) clang OS 🌸

Stable stage1-only build

LLD linker included

Polly optimizer enabled

Compiler-rt sanitizers

Multi-arch target ✅

Test compile & kernel build successful! 😻

Known Issues:

Extracting to /opt/ may require root 🐾

Ninja install errors can use manual install / DESTDIR workaround

Support / Donations:
If you like this toolchain and want to support its development, you can donate via:

Saweria: https://saweria.co/ucan
 🍵

Buy Me a Coffee: https://www.buymeacoffee.com/ucan
 ☕

Ko-fi: https://ko-fi.com/ucan
 💌

Trakteer: https://trakteer.id/ucan
 🍡

Every support makes the creator’s heart melt 🥹💖
Thank you so much~ 😘🌸

Wibu Words & Motivation:

Keep coding with warm tea 🍵💖

Don’t forget to rest 😽✨

Compiling is like cooking ramen: patience + love 🍜💖

Errors aren’t sad—they’re just the compiler smiling 😹💞

May your projects run smoothly, your heart be happy, and RAM stay fast 🐰💻💖

Have Fun & Keep Wibu Coding! 🌸
