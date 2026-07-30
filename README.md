# OpenVoiceOS Tray Indicator

A system tray application for **OpenVoiceOS**. It shows the assistant's current status and gives you a menu for quick interaction. It uses Python, GTK3, and AppIndicator3.

![image](https://github.com/user-attachments/assets/c6b7b884-f4e9-4af5-9415-9b292549bbd3)

---

## Features

* Shows the OpenVoiceOS status in the system tray. Status values include Listening, Speaking, Thinking, Sleeping, WakeWord, Errors, and Idle.
* Updates the tray icon title in real time. It reacts to [OpenVoiceOS message bus](https://github.com/OpenVoiceOS/ovos-bus-client) events.

The menu lets you:

* Start microphone listening.
* Stop the current OpenVoiceOS action.
* Type a query and send it to OpenVoiceOS as if you spoke it.
* Type text for OpenVoiceOS to speak.
* Quit the tray app.

---

## Requirements

* Python 3
* GTK 3, with Python GObject introspection bindings
* AppIndicator3 (Ubuntu or another Linux system with libappindicator support)
* The `ovos_bus_client` package from [OpenVoiceOS](https://github.com/OpenVoiceOS/ovos-bus-client)

---

## Usage

* The tray icon updates on its own, based on OpenVoiceOS events.
* Use the tray menu to control OpenVoiceOS or send text commands.
* To exit, select **Quit** in the menu, or press `Ctrl+C` in the terminal.

## Related projects

* [OpenVoiceOS/ovos-bus-client](https://github.com/OpenVoiceOS/ovos-bus-client): the message bus client this tray app connects to.
* [OpenVoiceOS/ovos-core](https://github.com/OpenVoiceOS/ovos-core): the OpenVoiceOS assistant this tray app controls.
