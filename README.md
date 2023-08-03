# DVWA-on-K3s

**Project Name**: Implementing and Securing a Kubernetes Cluster Running DVWA Containers

**Overview**: This project aims to demonstrate competence in using Kubernetes, Docker containers, and network security to set up a purposely vulnerable web server in a controlled, ethical environment. The goal is to explore and understand the potential vulnerabilities that can occur in real-world situations, and how to mitigate them.

**Objective**: Set up a Kubernetes Cluster running Docker containers of a purposely vulnerable web application (DVWA - Damn Vulnerable Web Application) and expose it to the open internet. This project will be done with a focus on creating a controlled and ethical testing environment that mimics real-world vulnerabilities.

**Procedure:**

**Hardware Preparation**

1. Obtain a Raspberry Pi 4 Model B. The version with 4GB of RAM should be sufficient.
2. Purchase the following peripherals: Micro SD card (32GB or more) x1, Ethernet cable x1, Micro HDMI to HDMI cable x1, USB-C power supply x1.
3. Once all the hardware is ready, install the Micro SD card into your Raspberry Pi, connect the Ethernet cable, the HDMI cable, and power it up with the USB-C power supply.


**Software Preparation**
(If following Pi installation procedure natively, skip to step 5)
1. Download the Raspberry Pi Imager from the Raspberry Pi website.
2. Use the Raspberry Pi Imager to write the "Raspberry Pi OS (32-bit)" to your Micro SD card.
3. After completing the write process, install the Micro SD card into the Raspberry Pi and power it up.
4. Follow the on-screen instructions to complete the Raspberry Pi OS setup.
5. Open a terminal and install Docker with `curl -sSL https://get.docker.com | sh`, then add the `pi` user to the `docker` group with `sudo usermod -aG docker pi`.
6. Install k3s, a lightweight Kubernetes distribution, using `curl -sfL https://get.k3s.io | sh -`.
7. Verify the correct installation of Kubernetes by executing `kubectl get nodes`.