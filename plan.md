```markdown
### Step 1: Initialize Frame Structure and Client State
```text
1. Create base HTML frame with empty state container
2. Implement client-side state initialization using localStorage
3. Set up CSS foundation for UI components

Files: index.html, style.css, client.js
```

### Step 2: Create Start/Stop Toggle Button UI
```text
1. Add toggle button to HTML with state-specific classes
2. Style button states (running/stopped) in CSS
3. Implement basic click handler skeleton

Files: index.html, style.css, client.js
```

### Step 3: Implement State Management for Tracking
```text
1. Connect button to localStorage state updates
2. Add start/stop timestamp handling
3. Implement state persistence methods

Files: client.js, stateManager.js (new)
```

### Step 4: Build Elapsed Time Display Component
```text
1. Create time display HTML element
2. Add real-time update mechanism using requestAnimationFrame
3. Implement HH:MM:SS formatting utility

Files: index.html, client.js, timeUtils.js (new)
```

### Step 5: Establish Daily Total Persistence
```text
1. Implement UTC midnight detection
2. Create daily total accumulation logic
3. Add localStorage cleanup scheduler

Files: timeUtils.js, client.js
```

### Step 6: Develop Progress Bar Animation System
```text
1. Add progress bar HTML structure
2. Create CSS animation rules
3. Connect animation state to tracking status

Files: index.html, style.css, client.js
```

### Step 7: Implement Server-Side Duration Validation
```text
1. Create edge function endpoint
2. Add duration computation logic
3. Set up client-server POST communication

Files: api/compute.js (new), client.js
```

### Step 8: Integrate Auto-Save Functionality
```text
1. Add interval-based save mechanism
2. Implement differential save optimization
3. Add visual save indicator

Files: client.js, style.css
```

### Step 9: Add State Integrity Checks
```text
1. Implement CRC32 checksum generation
2. Add state validation on load
3. Create auto-reset fallback

Files: stateManager.js (update), client.js
```

### Step 10: Implement Error Recovery UI
```text
1. Create error overlay component
2. Add state restoration controls
3. Style error notification system

Files: index.html, style.css, client.js
```