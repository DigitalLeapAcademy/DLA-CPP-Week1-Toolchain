# Week 1 Setup Guide: C++ Toolchain

Get your computer ready to compile and run C++ code.

---

## **Option A: Windows 10/11**

### **1. Install VS Code**
1. Download: https://code.visualstudio.com
2. Run installer → Check "Add to PATH" and "Register Code as an editor"

### **2. Install MinGW-w64 Compiler**
This gives us **g++**
1. Easiest: Open **Command Prompt** as Admin and run:
2. Or download from: https://www.mingw-w64.org/downloads/ → Install to `C:\mingw64`
3. **Add to PATH**: 
   Search "Environment Variables" → `Path` → `New` → Add `C:\mingw64\bin`
4. Restart Command Prompt and test: `g++ --version`

### **3. VS Code Extensions**
Open VS Code → Extensions `Ctrl+Shift+X` → Install:
1.  `C/C++` by Microsoft
2.  `Code Runner` by Jun Han

### **4. Test It**
1. Open `hello.cpp` from the root of this repo in VS Code
2. Open Terminal `Ctrl+~`
3. Compile: `g++ hello.cpp -o hello`
4. Run: `./hello`
You should see: `Hello from DigitalLeapAcademy!`

---

## **Option B: Mac**

### **1. Install Xcode Command Line Tools**
This gives us `g++` and `clang++`
1. Open `Terminal` from Spotlight
2. Run: `xcode-select --install`
3. Click "Install" → Agree → Wait

### **2. Install VS Code**
Download: https://code.visualstudio.com → Drag to Applications

### **3. VS Code Extensions**
Open VS Code → Extensions `Cmd+Shift+X` → Install:
1.  `C/C++` by Microsoft
2.  `Code Runner` by Jun Han

### **4. Test It**
1. Open `hello.cpp` from the root of this repo in VS Code
2. Open Terminal `Ctrl+~`
3. Compile: `g++ hello.cpp -o hello`
4. Run: `./hello`
You should see: `Hello from DigitalLeapAcademy!`

---

## **Troubleshooting**
- `g++: command not found` → PATH not set. Restart terminal/PC.
- Permission error on Mac → Run `chmod +x hello`
