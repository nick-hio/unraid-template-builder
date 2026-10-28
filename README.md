<h1 align="center">Unraid Template Builder</h1>
<p align="center">Interface to build Unraid Docker container templates.</p>

<div align="center">
  <a target="_blank" href="https://nick-hio.github.io/unraid-template-builder/">Open App</a> •
  <a target="_blank" href="https://github.com/nick-hio/unraid-template-builder">GitHub</a>
</div>

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/nick-hio/unraid-template-builder/refs/heads/main/screenshots/1-overview.png">
    <img src="https://raw.githubusercontent.com/nick-hio/unraid-template-builder/refs/heads/main/screenshots/1-overview.png" alt="Logo for Unraid Template Builder">
  </picture>
</p>

## Features

- Uses the same field names, order, and values from Unraid's [Docker manager](https://github.com/unraid/webgui).
- Paths, ports, variables, labels, and devices, with display, required, and mask options.
- Network types: bridge, host, container, none, and custom networks. Fixed IP and MAC addresses. Tailscale settings.
- CPU pinning, memory limit, extra parameters, and post arguments.
- Live XML preview with syntax highlighting.
- Copy to the clipboard, or download with a custom file name.
- Import an existing template with the Import button, or drag and drop an XML file onto the page.
- Work saves in the browser's local storage. Use the reset button to clear the data.

## Add Template to Unraid

1. Copy the XML file to `/boot/config/plugins/dockerMan/templates-user/` on your Unraid server.
2. In the Unraid web UI, go to **Docker** > **Add Container**.
3. Select the template from the **Template** list.

## Screenshots

> Visit [`/screenshots`](https://github.com/nick-hio/unraid-template-builder/tree/main/screenshots) for more.

- Runtime configuration:

<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/nick-hio/unraid-template-builder/refs/heads/main/screenshots/6-cpu-pinning.png">
    <img src="https://raw.githubusercontent.com/nick-hio/unraid-template-builder/refs/heads/main/screenshots/6-cpu-pinning.png" alt="Logo for Unraid Template Builder">
  </picture>
</p>

## License

MIT. See [LICENSE](LICENSE).
