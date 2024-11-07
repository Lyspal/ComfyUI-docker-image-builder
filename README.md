# ComfyUI-docker-image-builder

A containerization of the official ComfyUI diffusion model GUI. Includes ComfyUI-Manager.

## Goal

Originally, an attempt to containerize ComfyUI for deployment on a homelab and integration with an Open WebUI instance.

## Usage

1. Use the `install_ComfyUI.sh` or `install_ComfyUI.bat` (Windows) script to clone the repositories and install ComfyUI-Manager.
2. Build the Docker image by running `docker build -t comfyui .` in the root directory of this repository.
3. Run `docker compose up -d` to start the container.
4. Open your browser and go to `http://localhost:8188` to access the GUI.

## Known Issues

- Some more directories and files should probably be ignored during build.
- Permission issues with some scripts (e.g., ComfyUI-Manager) when running as non-root user in Docker.

## Disclaimer

This project is not affiliated with nor endorsed by ComfyUI, ComfyUI Manager, or their respective owners.

This project was created for my own personal use and educational purposes only. It is published with thw hope that it might be useful to others, but without any warranty of any kind, express or implied. Use at your own risk... as I myself am currently doing.

## Credits

- [confyanonymous/ComfyUI](https://github.com/comfyanonymous/ComfyUI)
- [ltdrdata/ComfyUI-Manager](https://github.com/ltdrdata/ComfyUI-Manager)

May this project shed a tiny little more light on the work of their authors.

Take a detour and go visit them at [comfyui.org](https://comfyui.org/).
