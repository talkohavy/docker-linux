# Dockerized Linux

A small **Linux environment in Docker** (Node Alpine) with **Git**.

## 1. Original Purpose

Environment you can `git clone` and `git pull` the same repos your Mac can, without copying keys into the image.

Useful when you want a consistent Linux toolchain or to experiment in a container, but still authenticate to Git over SSH exactly like on your machine—no duplicate key management inside the image.

## 2. Scripts

### - A. `build`

```bash
npm run build
```

Build image (docker-linux:latest).

### - B. `dev`

```bash
npm run dev
```

Runs a disposable Linux interactive shell, with `git`, `ssh`, and Corepack enabled.  
Your host `~/.ssh`, is mounted as read-only at `/root/.ssh`.
You **Git identity** (name / email) is set in the Dockerfile.
