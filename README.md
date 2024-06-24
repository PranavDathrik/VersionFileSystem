# VersionFileSystem
Versioning File System (C++)
The Versioning File System (VFS) is a simple filesystem implemented using FUSE (Filesystem in Userspace) that includes version control for files. Each time a file is written to, the old version is saved in a SQLite database. This allows users to retrieve and revert to previous versions of files.

Features:
Basic file operations: create, read, write, delete.
Version control: Each write operation saves the current version of the file.
Metadata management: Use SQLite to store metadata for versioning.
Command-line interface: Interact with the filesystem through standard file operations.
Dependencies:
libfuse3 for FUSE functionalities.
sqlite3 for SQLite database handling.
Instructions for Setting Up and Running the Project
Install Dependencies:

libfuse3: Install using your package manager (e.g., sudo apt-get install libfuse3-dev on Ubuntu).
SQLite3: Install using your package manager (e.g., sudo apt-get install libsqlite3-dev on Ubuntu).
