# SSH Project

![Project Badge](https://img.shields.io/badge/Project-Novice-blue)

## Table of Contents
1. [Project Overview](#project-overview)
2. [Learning Objectives](#learning-objectives)
3. [Project Requirements](#project-requirements)
4. [Tasks](#tasks)
5. [Resources](#resources)
6. [How to Run](#how-to-run)
7. [License](#license)

---

## Project Overview

This project involves setting up and connecting to a remote Ubuntu server using SSH. You'll generate an RSA key pair, configure SSH settings, and allow passwordless access. The project emphasizes learning server management basics and the secure connection process using SSH.

The server provided is configured with Ubuntu 20.04 LTS and is accessible through the intranet. Your server details, including IP and username, can be found in the "My Servers" section.

## Learning Objectives

By completing this project, you will learn:
- What a server is and where they are commonly located.
- What SSH is and its importance in secure connections.
- How to create and use an SSH RSA key pair for secure access.
- The benefits of using `#!/usr/bin/env bash` over `/bin/bash`.

## Project Requirements

- **Environment**: Ubuntu 20.04 LTS.
- **Editors**: vi, vim, emacs.
- **Bash Scripts**: Scripts must be executable, with each script beginning with `#!/usr/bin/env bash` followed by a comment describing the script’s functionality.
- **GitHub Repository**: `alu-system_engineering-devops`.
- **Directory**: `ssh`.

## Tasks

1. **Use a Private Key**  
   Write a Bash script to connect to the server with the private key `~/.ssh/school` as the `ubuntu` user.  
   **File**: `0-use_a_private_key`

2. **Create an SSH Key Pair**  
   Write a script that generates an RSA key pair.  
   - The private key should be named `school`.
   - The key should have 4096 bits and be protected by the passphrase `betty`.  
   **File**: `1-create_ssh_key_pair`

3. **Client Configuration File**  
   Configure your SSH client to use the private key `~/.ssh/school` and refuse password authentication.  
   **File**: `2-ssh_config`

4. **Add Public Key for Access**  
   Add a provided public key to the server’s authorized keys to enable access for others.

## Resources

- [What is a (physical) server?](#)
- [SSH Essentials](#)
- [Public Key Authentication for SSH](#)
- [Secure Shell Wiki](#)
- [RFC 4251 - SSH Protocol](https://datatracker.ietf.org/doc/html/rfc4251)

## How to Run

1. **Clone the Repository**
   ```bash
   git clone git@github.com:your-username/alu-system_engineering-devops.git
   cd alu-system_engineering-devops/ssh

