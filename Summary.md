# Chapter-1: What is eBPF, and why is it important?

Basic initial understanding of eBPF is that is allows for kernal level programs to be executed and dynamimcally modify Linux kernal
Advantages of kernal level programs:- 1. Fast 2. More Control

- BPF was used in 'tcpdump'
  (tcpdump listens on a network device to all incoming packets and logs them)
- eBPF maps are used to share information between kernal space and user space
- bpf() system call is used to interact with eBPF programs froom the user space
- eBPF verifier makes sure that eBPF programs are safe to run since we are running programs in kernal space hence it is extremely necessary

- 'kprobes' and 'hooks' in kernal
- 'BTF - BPF Type Format' makes eBPF programs much more portable
  (don't understand what it means yet)

The Linux Kernal:-

- Software layer between hardware and application
- syscall - system calls
- strace - shows all the sysytem calls an application makes

Dynamic Loadinng of eBPF Programsw:-

- eBPF programs can be dynamically loaded
- Don't need reboot
- Gains complete visibility as soon as program is loaded
  (extremely useful for cloud deployments)
