# Kernel Process Management Repository

This repository contains a collection of kernel modules illustrating various aspects of process management in the Linux Kernel. Each sub-directory represents a self-contained module with its associated files, focusing on different aspects of Kernel Process Management.

## Structure
```
.
├── 1_num_online_cpus
├── 2_print_tasks
├── 3_current
├── 4_current_tasks
├── 5_find_task
├── 6_vmarea
├── LICENSE
└── README.md
```

### Modules:
1. **1_num_online_cpus**
   - **Objective**: Demonstrates obtaining the number of online CPUs.
   - **Files**:
     - `online_cpus.c`: Source file
     - `Makefile`: Compilation instructions
     - `readme.md`: Module-specific instructions and information.
   
2. **2_print_tasks**
   - **Objective**: Illustrates enumerating over tasks in the system.
   - **Files**:
     - `tasks.c`: Source file
     - `Makefile`: Compilation instructions
     - `readme.md`: Module-specific instructions and information.
   
3. **3_current**
   - **Objective**: Demonstrates accessing the current task structure.
   - **Files**:
     - `current.c`: Source file
     - `Makefile`: Compilation instructions
     - `readme.md`: Module-specific instructions and information.
   
4. **4_current_tasks**
   - **Objective**: Explains the concepts behind current tasks in the kernel.
   - **Files**:
     - `tasks.c`: Source file
     - `Makefile`: Compilation instructions
     - `readme.md`: Module-specific instructions and information.
   
5. **5_find_task**
   - **Objective**: Provides a way to find a task with a given PID.
   - **Files**:
     - `tasks.c`: Source file
     - `Makefile`: Compilation instructions
     - `readme.md`: Module-specific instructions and information.
   
6. **6_vmarea**
   - **Objective**: Explains the process memory management concepts in the kernel.
   - **Files**:
     - `tasks.c`: Source file
     - `Makefile`: Compilation instructions
     - `readme.md`: Module-specific instructions and information.

### Getting Started

To build and load a module, navigate to the corresponding directory and execute the following commands:

```sh
make          # to build the module
sudo insmod <module_name>.ko   # to insert the module into the kernel
```

To remove the module from the kernel and clean the directory, execute:

```sh
sudo rmmod <module_name>   # to remove the module from the kernel
make clean    # to clean the directory
```

### License

This project is licensed under the terms of the included [LICENSE](./LICENSE) file.

### Acknowledgments

We would like to extend our gratitude to all contributors and developers who have worked on understanding and elucidating the concepts behind kernel process management, making this repository possible.

---

Please refer to individual `readme.md` files within each module's directory for more specific details and usage instructions pertaining to that module.