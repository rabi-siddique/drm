When working with Docker, I often find myself repeatedly running `docker ps` to identify the container ID that I need to remove. This process involves manually copying the container ID and then pasting it into the `docker rm` command — a step I find particularly tedious.

# How `drm` works

I've developed a custom script that helps a little with my productivity by eliminating the need for copy-pasting! 😄

I've developed a custom script that enhances a little bit of my productivity by
saving me a Copy Paste :D . Here’s how it improves my workflow:

- `View Containers`: I start by listing all active containers with docker ps.
- `Select a Container`: Instead of copying IDs, I simply note the position of the container in the list, which is much quicker.
- `Run My Script`: With the command `drm <Number>`, where `<Number>` is the sequence number of the container, I can remove it directly. No ID copying needed.
- `Container Removed`: Just like that, the container is gone, putting a little less friction on my brain! 😂

# Download and Install

- Download the Script

  ```bash
  sudo curl -o /usr/local/bin/drm https://raw.githubusercontent.com/rabi-siddique/drm/refs/heads/main/drm
  ```

- Make the Script Executable

  ```bash
  sudo chmod +x /usr/local/bin/drm

  ```

- Usage
  ```bash
  drm <Container_Number>
  ```

# OS

- `MacOS`: The script has been tested on macOS and should work as expected.
- `Linux`: If you encounter any issues on Linux, please report them to help improve the script.
