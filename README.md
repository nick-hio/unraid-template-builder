# Unraid Template Builder

Interface to build Unraid Docker container XML templates.

Uses the same field names, order, and values from Unraid's [Docker manager](https://github.com/unraid/webgui).

## Usage

Get started by visiting the [GitHub Pages site](https://nick-hio.github.io/unraid-template-builder/) or by downloading and opening `index.html` in your browser.

## Features

- Paths, ports, variables, labels, and devices, with display, required, and mask options.
- Network types: bridge, host, container, none, and custom networks. Fixed IP and MAC addresses. Tailscale settings.
- CPU pinning, memory limit, extra parameters, and post arguments.
- Live XML preview with syntax highlighting.
- Copy to the clipboard, or download with a custom file name.
- Import an existing template with the Import button, or drag and drop an XML file onto the page.
- Work saves in the browser's local storage. Use the reset button to clear the data.

## Add the template to Unraid

1. Copy the downloaded file to `/boot/config/plugins/dockerMan/templates-user/` on your Unraid server.
2. In the Unraid web UI, go to **Docker** > **Add Container**.
3. Select the template from the **Template** list.

## License

MIT. See [LICENSE](LICENSE).
