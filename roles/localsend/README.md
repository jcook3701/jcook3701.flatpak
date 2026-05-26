# Localsend

[LocalSend](https://github.com/localsend/localsend) is a cross-platform app that enables secure communication between devices using a REST API and HTTPS encryption. Unlike other messaging apps that rely on external servers, LocalSend doesn't require an internet connection or third-party servers, making it a fast and reliable solution for local communication.

Install **Localsend** package from flathub.

``` shell
$ ansible-playbook jcook3701.flatpak.localsend.yml
```

Uninstall **Localsend** package from flathub.

``` shell
$ ansible-playbook jcook3701.flatpak.localsend.yml -K -e "localsend_state=absent"
```
