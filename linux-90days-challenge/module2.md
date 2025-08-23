# Linux Architecture  

Linux is divided into two main parts: Kernel Space and User Space.  
This separation ensures stability, security, and efficient resource management.  

---

 1. Kernel Space vs User Space  

- Kernel Space  
  - The core of the operating system.  
  - Directly interacts with hardware (CPU, memory, disk, network).  
  - Provides low-level services like process scheduling, memory allocation, and device drivers.  

- User Space  
  - Where applications and user programs run.  
  - Examples: Shell (`bash`), text editors (`vim`, `nano`), and services (web servers).  
  - User programs cannot directly access hardware → they must request services from the kernel.  

---

 2. System Calls  

- A bridge between User Space and Kernel Space.  
- Applications request resources or services from the kernel using system calls.  
- Example system calls:  
  - `open()` → open a file  
  - `read()` → read data  
  - `write()` → write data  
  - `close()` → close file  

---

 3. Init Systems  

The init system is the first process started by the kernel during boot. It manages services and background processes.  

- SysVinit (Old system)  
  - Starts processes one after another (sequential).  
  - Slower boot times.  

- systemd (Modern system)  
  - Starts services in parallel → faster boot.  
  - Can monitor and restart services automatically.  
  - Common in modern Linux distributions (Ubuntu, CentOS, RHEL, Fedora).  

---

 4. Process Creation  

- `fork()`  
  - Creates a child process by duplicating the parent process.  
  - Both processes can run independently.  

- `exec()`  
  - Replaces the process memory with a new program.  
  - Used after `fork()` to start a completely new process.  

---

👉 Why important?  
Understanding Linux architecture is critical in DevOps & Cloud because it explains:  
- How Linux boots up  
- How applications talk to the kernel  
- How processes are created and managed  
- How services (like web servers, databases, containers) are started and monitored  
