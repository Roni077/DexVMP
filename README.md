# DexVMP: Advanced Dalvik Bytecode Protection 🛡️

![DexVMP Banner](image.webp)

Run and protect Dalvik bytecode using advanced dex virtualization technology. DexVMP transforms your APK into a highly secured application through innovative virtualization techniques.

## ✨ Key Features

- **Virtualization Technology**: Execute Dalvik bytecode in a custom VM environment
- **String Encryption**: Random string obfuscation for enhanced security
- **Customizable VM**: Tailor VM class names, library names, and registration
- **Synthetic Method Protection**: Advanced protection for synthetic methods
- **NDK Integration**: Seamless integration with Android NDK toolchain

## 🚀 Quick Start

### Prerequisites

- Termux environment
- Android NDK (automatic installation supported)

### Automated NDK Installation

```bash
cd && pkg upgrade && pkg install wget && \
wget https://github.com/Roni077/dexvmp/raw/master/termux-ndk.sh \
--no-verbose --show-progress -N && \
chmod +x termux-ndk.sh && \
bash termux-ndk.sh
```

### Environment Setup

```bash
export SDK_PATH=/data/user/0/com.termux/files/home/android-sdk
export NDK_PATH=/data/user/0/com.termux/files/home/android-sdk/ndk/25.2.9519653
export CMAKE_PATH=/data/user/0/com.termux/files/home/android-sdk/cmake/3.22.1
```

## 🔧 Usage

### Terminal Execution (Termux)

![Execution Example](image2.webp)

```bash
bash start-vm.sh
```

### Console Execution

```bash
java -jar vm-protect.jar apk input.apk convertRules.txt mapping.txt
```

## ⚙️ Customization Options

1. **Merge VM Library** - Combine VM libraries for optimized performance
2. **Random String Encryption** - Advanced string obfuscation techniques
3. **Custom VM Class Name** - Specify your own VM class identifier
4. **Custom VM Library Name** - Personalize the VM library name
5. **Custom VM Registration** - Unique registration naming
6. **Synthetic Method Protection** - Enhanced protection for synthetic methods

## 📚 Technical Details

DexVMP utilizes advanced bytecode virtualization to protect your Android applications from reverse engineering and tampering. The solution creates a custom execution environment that makes static analysis extremely challenging.

## 🔗 Project Origins

This project is based on the excellent work of [nmmp](https://github.com/maoabc/nmmp) by maoabc, enhanced with additional security features and improvements.

---

**Note**: Ensure you have sufficient storage space before installation as the NDK and toolchain require significant disk space.

For support and contributions, please refer to the original project repository and check existing issues before submitting new ones.
