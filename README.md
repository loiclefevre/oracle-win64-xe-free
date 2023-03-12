# Oracle win64 XE and Free

This repository demonstrates technics to reduce both the size of the Oracle database for windows XE and Free, as well as the duration to install it.

# Technics

It starts all from a standard installation and build from this a 7zip self-extracting archive.

## Size reduction
- Remove unused files
- Reduce database files footprint
- Create a solid archive compressed with Ultra LZMA2 algorithm

## Install duration reduction
- Start from an standard installation
- Reduce overall disk size
- Provide a shell script that proceed with all the final installation steps
    - Windows registry update (including SYSTEM PATH environment variable)
    - Windows services creation
    - Listener and Database launch
    - Create XEPDB1 at the end
