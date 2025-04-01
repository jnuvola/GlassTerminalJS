# GlassTerminalJS
A customizable, glass-styled vintage terminal component for web applications.

### Configuration Options

You can customize the terminal by passing options to the constructor:

```javascript
const terminal = new GlassTerminal({
  containerId: 'terminal-container',  // ID of the container element
  width: 500,                         // Width in pixels
  height: 500,                        // Height in pixels
  fontSize: 11,                       // Font size in pixels
  terminalColor: '#33ff33',           // Terminal text color
  autoRestart: true,                  // Whether to restart after completion
  lines: [                            // Content to display
    '> Hello, world!',
    '> Running system check...',
    '> All systems operational.'
  ]
});
```

### API Methods

```javascript
// Mount the component to the DOM
terminal.mount();

// Start the typing animation
terminal.start();

// Pause the animation
terminal.stop();

// Clear the terminal and reset to initial state
terminal.reset();

// Change the content displayed
terminal.updateLines([
  '> New content line 1',
  '> New content line 2'
]);
```
