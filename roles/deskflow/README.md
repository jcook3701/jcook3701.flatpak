# Deskflow

[Deskflow](https://github.com/deskflow/deskflow) is a free and open source keyboard and mouse sharing app. Use the keyboard, mouse, or trackpad of one computer to control nearby computers, and work seamlessly between them. It's like a software KVM (but without the video). TLS encryption is enabled by default. Wayland is supported. Clipboard sharing is supported.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `deskflow_state` | str | The desired deployment state of the Deskflow Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `deskflow_package` | str | The Flatpak application identifier for Deskflow. | `"org.deskflow.deskflow"` |
| `deskflow_remote_name` | str | The name of the remote repository hosting the Deskflow Flatpak package. | `"flathub"` |

## Authors Notes

Deskflow installed with flatpak is installed within the user space.  This means that this is not a viable solution if you need Deskflow to operate before login.

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
