# Profile Card — Sprint 3

React Native / Expo solution based on the supplied Task 3 student starter.

## Run

```sh
npm ci
npm start
```

On Windows PowerShell, use `npm.cmd` if script execution is blocked. Start your Android emulator and press `a` in the Expo terminal, or scan the QR code with a compatible Expo Go app on a phone connected to the same Wi-Fi.

## Features

- Share profile opens a modal with a scrollable list of eight contacts.
- Select or deselect contacts; sharing is disabled until at least one is selected.
- Confirming shows a native alert with the selected names and closes the modal. This is a simulation; no messages are actually sent.
- Cancel, the dark backdrop and Android Back close the modal and clear its selection.
- Five recent projects scroll horizontally.
- SafeAreaProvider and SafeAreaView protect the main screen.
- Follow, messaging, bio expansion, online status and skill selection from Task 2 remain available.

All mandatory steps are included. Optional bonus features are not included. Native alerts and Android Back should be tested in Expo Go or an emulator, not only in the browser.

The seven checkpoint answers are in [ANSWERS.md](ANSWERS.md).

## Submission

The branch is `task/modals-scrollview-safearea`, with one commit per step. Open a Pull Request and attach screenshots or a short recording showing the projects and the contact selection modal.
