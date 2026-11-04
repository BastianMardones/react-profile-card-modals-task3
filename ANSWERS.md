# Checkpoint answers

1. `visible` determines whether the modal is displayed. We control it with `useState` because opening or closing the dialog changes the interface and must trigger a new render.

2. `onRequestClose` handles a system request to dismiss the modal, such as the Android back button. If its handler does not set visibility to false, the modal stays open when the user presses back.

3. `transparent={true}` lets the underlying screen remain visible through transparent parts of the modal, while our overlay darkens it. The three animation types are `none`, `slide` and `fade`.

4. `ScrollView` makes content accessible when it exceeds the available space; an ordinary View does not provide scrolling and its overflowing content can become inaccessible. For a large or unbounded list, choose `FlatList`, which renders a window of items rather than mounting every child at once.

5. `style` controls the ScrollView itself, such as its visible height, border and background. `contentContainerStyle` controls the inner container surrounding its children, including spacing, padding and alignment.

6. `SafeAreaView` adds spacing to keep content away from device cutouts and system interface areas, such as the status bar and gesture area. We use `react-native-safe-area-context` for cross-platform support and place a `SafeAreaProvider` at the root to supply the inset information.

7. Use a single modal for a short, focused action, keep ScrollView lists small (five projects and eight contacts here), and protect screen content with a safe area. A long multi-step registration form would be better on its own screen than inside a modal.
