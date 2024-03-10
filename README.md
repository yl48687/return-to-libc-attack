# return-to-libc
The project utilizes the Return-to-libc Attack Lab provided by SEEDLAB 2.0 as a foundational platform for exploration and experimentation in the domain of network security. This lab offers an investigation into an intriguing variant of buffer-overflow attacks, capable of circumventing existing protection schemes deployed in major Linux operating systems. Unlike traditional buffer-overflow exploits that rely on executing malicious shellcode injected into the stack, this variant, known as Return-to-libc, leverages existing code fragments within the libc library to achieve its objectives.

The primary learning objective of this lab is to provide a firsthand understanding and execution experience of Return-to-libc attacks. By exploiting buffer-overflow vulnerabilities in a given program, the exploration delves into the intricacies of crafting and executing Return-to-libc exploits to gain root privileges.

One of the fundamental protections against buffer-overflow attacks is the implementation of non-executable stacks in operating systems. However, Return-to-libc attacks demonstrate the limitations of this approach by bypassing the need for an executable stack altogether. Instead, these attacks manipulate the program's control flow to execute predefined functions, such as system calls, from the libc library.

## Report
The detailed project report, including the methodology, findings, and analysis of Return-to-libc attack techniques and countermeasures, can be accessed in the attached `Report.pdf`.

## Additional

### Original Lab Instructions
The original lab instructions outlining the objectives, tasks, and guidelines for the Return-to-libc Attack Lab can be accessed [here](https://seedsecuritylabs.org/Labs_20.04/Software/Return_to_Libc/).

### Modified Files
The modified files according to lab instructions are as follows:
- `exploitT3.py`
─ `exploitT4.py`
─ `exploitT5.py`

The original (non-modified) files can be found in the `Labsetup` directory within this repository.

## File Structure and Content
```
return-to-libc/
├── exploitT3.py
├── exploitT4.py
├── exploitT5.py
├── Labsetup/
│   ├── exploit.py
│   ├── Makefile
│   └── retlib.c
├── README.md
└── Report.pdf
```