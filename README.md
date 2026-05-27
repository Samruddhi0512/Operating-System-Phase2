# 💻 Operating System Phase 2 Simulator

## 📌 Project Overview

This project is a simple **Operating System Phase-2 Simulator** developed in **C++**.  
It is an advanced version of the Operating System Phase-1 project and demonstrates important operating system concepts such as:

- 🧠 Memory Management
- ⚡ Interrupt Handling
- 📂 Job Processing
- 🔁 Instruction Execution Cycle
- 📥 Input/Output Operations
- ⏱️ Time Limit Handling
- ❌ Error Detection and Handling

The simulator reads jobs from an input file, loads them into memory, executes instructions sequentially, handles interrupts, and stores the output in an output file.

---

# 🛠️ Technologies Used

- **Language:** C++
- **Compiler:** g++ / MinGW
- **IDE:** VS Code
- **Concepts:** Operating System, Memory Management, Interrupt Handling

---

# 📂 Project Structure

```bash
SAMRUDDHI'S-OS-PHASE02/
│
├── phase2.cpp              # Main source code
├── input.txt               # Input instructions and jobs
├── output.txt              # Generated output
├── OS-PHASE2.pdf           # Project documentation/report
├── phase2.exe              # Compiled executable file
│
└── .vscode/
    ├── c_cpp_properties.json
    ├── launch.json
    └── settings.json
```

---

# ✨ Features

✅ Simulates an Operating System environment  
✅ Supports multiple job execution  
✅ Implements interrupt handling  
✅ Performs memory management  
✅ Handles time and line limits  
✅ Executes instructions sequentially  
✅ Supports file input and output operations  
✅ Detects and handles errors efficiently  

---

# 📖 Control Cards Used

| Control Card | Description |
|--------------|-------------|
| `$AMJ` | Start of Job |
| `$DTA` | Start of Data |
| `$END` | End of Job |

---

# 📖 Instructions Supported

| Instruction | Description |
|--------------|-------------|
| `GD` | Get Data |
| `PD` | Print Data |
| `LR` | Load Register |
| `SR` | Store Register |
| `CR` | Compare Register |
| `BT` | Branch if True |
| `H`  | Halt Execution |

---

# 🧠 Memory Organization

The simulator uses:

- `M[100][4]` → Main Memory
- `IR[4]` → Instruction Register
- `R[4]` → General Register
- `IC` → Instruction Counter
- `C` → Toggle/Condition Flag

---

# ⚡ Interrupt Handling

## 🔹 Program Interrupts (PI)

- Operation Code Error
- Operand Error
- Invalid Page Fault

## 🔹 Service Interrupts (SI)

- Read Operation
- Write Operation
- Halt Operation

## 🔹 Time Interrupts (TI)

- Time Limit Exceeded

---

# ⚙️ Working of the Program

## 1️⃣ Initialization

Memory and registers are initialized with default values.

## 2️⃣ Loading Phase

Jobs and instructions are loaded from `input.txt` into memory.

## 3️⃣ Execution Phase

Instructions are fetched and executed one by one.

## 4️⃣ Interrupt Handling

The system checks for program, service, and time interrupts during execution.

## 5️⃣ Output Generation

The final output is stored in `output.txt`.

---

# 📥 Sample Input

```txt
$AMJ
GD10
PD10
H
$DTA
HELLO WORLD
$END
```

---

# 📤 Sample Output

```txt
HELLO WORLD
```

---

# ▶️ How to Run the Project

## 🔹 Step 1: Compile the Code

```bash
g++ phase2.cpp -o phase2
```

## 🔹 Step 2: Run the Program

### 💻 For Linux / Mac

```bash
./phase2
```

### 🪟 For Windows

```bash
phase2.exe
```

---

# 🎯 Concepts Demonstrated

This project helps in understanding:

- Operating System Design
- Job Processing
- Memory Simulation
- Interrupt Handling
- Error Handling
- File Handling in C++
- Register Operations
- Execution Cycle

---

# 🖥️ Output Example from Project

```txt
HELLO WORLD
PROGRAM EXECUTED SUCCESSFULLY
```

---

# 🚀 Future Improvements

Possible enhancements for future phases:

- Paging Mechanism
- Virtual Memory
- CPU Scheduling Algorithms
- Multiprogramming
- Process Synchronization
- Deadlock Handling
- Dynamic Memory Allocation

---

# 📚 Learning Outcomes

By completing this project, the following concepts were understood:

- How operating systems manage jobs
- Working of interrupts in OS
- Memory and register management
- Instruction execution cycle
- Error detection and handling
- File handling operations

---

# 👩‍💻 Author

**Samruddhi Bate**  
Computer Engineering Student

---





# 📜 License

This project is created for educational and academic purposes.
