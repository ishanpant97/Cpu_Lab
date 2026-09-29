# ⚡ CPU Architecture Lab

An interactive, educational computer architecture simulator suite running entirely in the browser with zero dependencies. Explore hardware internals from micro-step fetch-decode-execute cycles up to a complete Intel 8086 microprocessor simulation.

---

## 🌟 Included Modules

1. **⚙️ Custom 8-bit CPU Simulator**
   - Accumulator-based micro-architecture with 64-byte RAM.
   - Microcoded state machine with **Fetch → Decode → Execute** micro-stepping.
   - Live hardware dataflow diagram highlighting active busses (PC, MAR, MDR, ALU).
   - Preloaded programs: Series Sum, 3×4 Multiplication, 4! Factorial, Fibonacci Series, and Bitwise Logic.
   - Editable memory cells and output port logging.

2. **🔀 Memory Organisation & Endianness Lab**
   - Side-by-side comparison of **Big-Endian** (Network/RISC) vs **Little-Endian** (Intel x86).
   - Dynamic 8-bit, 16-bit, 32-bit, and 64-bit word sizing.
   - Interactive 64-byte RAM with single-byte and multi-byte read/write operations.
   - Presets for 32-bit hex, IPv4 addresses, and ASCII strings.

3. **💻 Full Assembly Interpreter**
   - 16-bit registers: `AX`, `BX`, `CX`, `DX`, `SI`, `DI`, `BP`, `SP`.
   - 8-bit mirrored sub-registers: `AL`, `AH`, `BL`, `BH`, `CL`, `CH`, `DL`, `DH`.
   - Flags register: `ZF`, `SF`, `CF`, `OF`, `PF`.
   - Stack instructions: `PUSH`, `POP`, `CALL`, `RET`.
   - Arithmetic, logic, shifts, rotations, comparison, and conditional branches.

4. **🎯 Addressing Modes Interactive Visualizer**
   - Immediate, Register, Direct, Register Indirect, Indexed, Based, Based-Indexed with Displacement, and Relative Addressing.
   - Animated 5-step hardware pipeline (Fetch → Decode → EA Math → Bus Transfer → Writeback).
   - Live RAM map highlighting the calculated Effective Address (EA).

5. **⚡ Intel 8086 Microprocessor Architecture Simulator**
   - Segment Registers: `CS`, `DS`, `SS`, `ES` with real 20-bit physical address generation (`Segment × 16 + Offset`).
   - Bus Interface Unit (BIU) cycle logger tracking Memory Reads, Writes, Stack pushes/pops, and odd-address misalignment cycles.
   - Subroutine calls via `SS:SP` stack frames.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| **`F8`** | Step forward one instruction |
| **`Space`** or **`F9`** | Run / Pause execution |
| **`F2`** | Assemble and Reset current simulator |
| **`1` – `5`** | Switch between Lab Tabs (1 to 5) |

---

## 🚀 How to Host on Vercel (100% Free)

This project is fully static (HTML, CSS, JavaScript) and requires **no build step**. It deploys to Vercel in under 60 seconds!

### Method 1: Deploy via GitHub (Recommended & Automatic)

1. **Commit and push to a new GitHub repository**:
   ```bash
   git add .
   git commit -m "Initial commit: CPU Architecture Lab"
   git branch -M main
   # Create a new repository on https://github.com/new and run:
   git remote add origin https://github.com/<YOUR_USERNAME>/cpu-architecture-lab.git
   git push -u origin main
   ```

2. **Deploy on Vercel**:
   - Go to [vercel.com](https://vercel.com) and log in (or sign up with GitHub).
   - Click **"Add New..." → "Project"**.
   - Select your `cpu-architecture-lab` repository and click **Import**.
   - In **Project Settings**:
     - *Framework Preset*: **Other** (detected automatically)
     - *Root Directory*: `./`
     - *Build Command*: Leave empty
     - *Output Directory*: Leave empty
   - Click **Deploy**!
   - Your site will be live instantly with a free `https://*.vercel.app` URL and automatic updates every time you push code!

---

### Method 2: Deploy directly via Vercel CLI

If you have Node.js / npm installed:
```bash
# In the project directory:
npx vercel
```
Follow the 3 quick prompts (use defaults), and your deployment URL will be generated immediately!

---

### Method 3: Drag & Drop via Vercel Dashboard

1. Zip or upload this folder directly to the [Vercel Dashboard](https://vercel.com/new).
2. It will deploy as a static website instantly.

---

## 📄 License
MIT License. Free for educational and personal use.
