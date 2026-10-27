# Unraid Template Builder

Interface to build Unraid Docker container XML templates.

## Usage

Get started by opening visiting the [GitHub Pages site](#) or by downloading `index.html` and opening it in your browser.

## Features

- Every field that Unraid's Docker manager writes to a user template.
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

## Field reference

The field names, order, and allowed values come from Unraid's Docker manager source code ([`unraid/webgui`](https://github.com/unraid/webgui), `emhttp/plugins/dynamix.docker.manager/include/`).

Unraid ignores fields that its version doesn't know, so newer fields such as `ExtraNetworks` and `MyMAC` are safe on older versions.

## License

MIT. See [LICENSE](LICENSE).
