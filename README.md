# Unraid Template Builder

A single HTML page that builds Unraid Docker container XML templates. Fill in the form, then copy the XML or download it as `my-<name>.xml`.

Everything runs in the browser. Nothing is sent to a server.

## Use it

Open `index.html` in a browser. No build step is needed.

You can also serve it with any static web server, or with GitHub Pages.

## Features

- Every field that Unraid's Docker manager writes to a user template, in the same order.
- Paths, ports, variables, labels, and devices, with display, required, and mask options.
- Network types: bridge, host, container, none, and custom networks. Fixed IP and MAC addresses.
- CPU pinning, memory limit, extra parameters, and post arguments.
- Tailscale settings, with the same option rules as Unraid.
- Live XML preview with syntax highlighting.
- Info icons beside the fields. Hover or focus one to see what the field does.
- Copy to the clipboard, or download with a custom file name. The name always starts with `my-`.
- Import an existing template with the Import button, or drag and drop an XML file onto the page.
- Your work saves in the browser's local storage.

## Add the template to Unraid

1. Copy the downloaded file to `/boot/config/plugins/dockerMan/templates-user/` on your Unraid server.
2. In the Unraid web UI, go to **Docker** > **Add Container**.
3. Select the template from the **Template** list.

## Field reference

The field names, order, and allowed values come from Unraid's Docker manager source code ([`unraid/webgui`](https://github.com/unraid/webgui), `emhttp/plugins/dynamix.docker.manager/include/`). Unraid ignores fields that its version does not know, so newer fields such as `ExtraNetworks` and `MyMAC` are safe on older versions.

## License

MIT. See [LICENSE](LICENSE).
