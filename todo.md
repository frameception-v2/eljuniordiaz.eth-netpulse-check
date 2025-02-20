```markdown
### Core
[x] 1. Create base HTML frame with empty state container  
**Validation:** Verify container exists in DOM via browser inspector  
**Files:** src/components/Frame.tsx

[ ] 2. Implement client-side state initialization using localStorage  
**Validation:** `localStorage.getItem('trackerState')` returns valid object  
**Files:** client.js

[ ] 3. Set up CSS foundation for UI components  
**Validation:** Body background and container padding visible  
**Files:** style.css

[ ] 4. Create state persistence methods in stateManager.js  
**Validation:** Manual state edits persist through page reload  
**Files:** stateManager.js

[ ] 5. Implement UTC midnight detection and daily rollover  
**Validation:** New day creates fresh dailyTotal entry  
**Files:** timeUtils.js

[ ] 6. Add CRC32 checksum generation for state validation  
**Validation:** Tampered state triggers console warning  
**Files:** stateManager.js

### API
[ ] 1. Create edge function endpoint for duration validation  
**Validation:** GET request returns 501 Not Implemented  
**Files:** api/compute.js

[ ] 2. Implement server-side timestamp validation  
**Validation:** Returns 400 for invalid time ranges  
**Files:** api/compute.js

### UI
[ ] 1. Add toggle button with .running/.stopped classes  
**Validation:** Button visually changes on class toggle  
**Files:** index.html, style.css

[ ] 2. Connect button click to state toggle (no persistence)  
**Validation:** Click changes button state temporarily  
**Files:** client.js

[ ] 3. Create animated time display container  
**Validation:** Shows 00:00:00 on initial load  
**Files:** index.html, client.js

[ ] 4. Implement requestAnimationFrame update loop  
**Validation:** Time updates every second (±50ms)  
**Files:** client.js

[ ] 5. Add progress bar with pauseable CSS animation  
**Validation:** Animation freezes when tab inactive  
**Files:** style.css, client.js

[ ] 6. Create floating save indicator component  
**Validation:** Briefly appears after localStorage.setItem  
**Files:** style.css, client.js

[ ] 7. Build error overlay with restoration controls  
**Validation:** forceReload() clears broken state  
**Files:** index.html, client.js
```

**Dependency Flow:**  
1. Core foundation → API endpoints → UI components  
2. State persistence before UI interactions  
3. Time utilities before progress animations  
4. Validation systems after core persistence  

**Critical Path:**  
HTML Frame → State Init → Button Wiring → Time Display → API Integration
