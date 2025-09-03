# Linux Cgroup Resource Hog 🐷

This is a simple Go program that **hogs CPU and RAM** so that you can test  
Linux Control Groups (cgroups v2) for resource limits.

---

## 🛠 Build Instructions

```bash
# Install Go (Debian/Ubuntu)
sudo apt update && sudo apt install -y golang

# Or RHEL/CentOS
sudo yum install -y golang

# Clone the repo
git clone https://github.com/sekanderdany/linux-cgroup-hog.git
cd linux-cgroup-hog

# Build
go build -o hog hog.go

# Run
./hog

## ⚠️ Warning

This program will consume all CPU cores and allocate 10MB of memory every second.

Use it only on test/lab VMs, never on production servers.

Stop with CTRL+C.

## 📚 Reference

This repo was created while practicing Linux cgroups examples inspired by
Iximiuz Labs and Ivan Velichko.

---