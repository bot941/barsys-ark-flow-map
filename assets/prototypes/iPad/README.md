# Barsys FTUE & Flow Prototypes

## Files Created

All 7 HTML prototype files have been rebuilt from scratch using the EXACT design DNA from NavMap2_Dark.html.

### 1. BLE_Dark.html (6 screens)
- **ble-search**: Searching for station with animated ring
- **ble-connecting**: Connecting to BARSYS-2849 with progress bar
- **ble-connected**: Success state with checkmark
- **ble-lost**: Connection lost error with action buttons
- **ble-reconnect**: Reconnecting attempt with animated ring
- **ble-manual**: Manual setup instructions with step cards

### 2. ErrNetwork_Dark.html (6 screens)
- **err-no-wifi**: WiFi connection lost
- **err-weak**: Weak WiFi signal warning
- **err-ble-drop**: Bluetooth disconnected
- **err-auth-expired**: Session expired, sign in required
- **err-relogin**: Login form with email/password
- **err-resolved**: Connection restored success state

### 3. ErrAI_Dark.html (6 screens)
- **err-ai-down**: AI service unavailable
- **err-pour-fail**: Pour interrupted with status card
- **err-station-off**: Station offline error
- **err-calibrate**: Calibration needed with steps
- **err-bottle-empty**: Empty bottles list with level bars
- **err-resolved**: Issue resolved success state

### 4. RecipeFlow_Dark.html (8 screens)
- **discover**: Recipe discovery with search and filter chips
- **filters**: Refined search with multiple chip groups
- **recipe-detail**: Split-layout recipe card with ingredients
- **confirm-pour**: Ready to pour confirmation dialog
- **pouring**: Active pour with circular progress
- **pour-complete**: Completed drink with ratings
- **rate**: Drink rating form with stars
- **share**: Social sharing interface

### 5. StationMgmt_Dark.html (7 screens)
- **station-home**: Station hub with stat cards and action items
- **bottles**: Bottle management with level indicators
- **add-bottle**: Add new bottle form
- **clean-start**: Start cleaning confirmation
- **clean-progress**: Cleaning progress indicator
- **maintenance**: Maintenance log with diagnostics
- **firmware**: Firmware update information

### 6. DeviceSetup_Dark.html (8 screens)
- **setup-welcome**: Welcome screen with gold orb
- **setup-power**: Power on instructions
- **setup-wifi**: WiFi network selection
- **setup-ble**: Bluetooth station discovery
- **setup-calibrate**: Calibration progress
- **setup-first-pour**: First pour test
- **setup-complete**: Setup complete success
- **setup-tips**: Quick tips grid

### 7. GuestMode_Dark.html (7 screens)
- **guest-scan**: QR code scanning frame (no context bar)
- **guest-welcome**: Welcome to party
- **guest-menu**: Drink selection grid (no context bar)
- **guest-order**: Order confirmation with ingredients
- **guest-queue**: Queue position display
- **guest-ready**: Drink ready notification
- **guest-rate**: Drink rating form

## Design DNA Applied

All files strictly adhere to the accepted NavMap2_Dark.html design language:

### CSS Variables (Exact Values)
```
--bg:#050505 (true black)
--s1:#0A0A0A, --s2:#111111, --s3:#191919 (grays)
--gold:#C8A97E, --gold-l:#E8D5B5 (gold variants)
--gold-d:rgba(200,169,126,0.08) (gold overlay)
--t1:#FFFFFF (white text)
--t2:rgba(255,255,255,0.55), --t3:rgba(255,255,255,0.25), --t4:rgba(255,255,255,0.10)
--glass:rgba(255,255,255,0.025) (glass backdrop)
--glass-b:rgba(255,255,255,0.04) (glass border)
--success:#7A9A82, --warning:#B8A67A, --error:#A07272
```

### Device Frame
- 1194px x 834px
- 22px border-radius
- Exact box-shadow: `0 0 0 1px rgba(255,255,255,0.03),0 80px 200px rgba(0,0,0,0.95)`

### Typography
- Font: Plus Jakarta Sans via @import
- Titles: 40px font-weight:200 letter-spacing:-1px
- Section labels: 9px letter-spacing:4px (NOT 6px or 8px)
- Strong text: font-weight:700

### Component Patterns
- Glass cards: padding:28px border-radius:20px
- Buttons: padding:16px 48px border-radius:14px
- Feature items: padding:14px border-radius:14px
- Feature thumbs: 44px x 44px border-radius:11px
- SVG stroke-width: 1px for content, 1.5px for navigation

### Animations (All Included)
- fadeScale, fadeIn, fadeUp, breathe, pulse
- sparkleFloat, slideUp, haptic

### Context Bar (Where Applicable)
- blur(40px) backdrop
- padding:0 32px 20px
- gradient: linear-gradient(to top,var(--bg) 70%,transparent)
- Navigation tabs with active state

## Screen Organization

Each file uses:
- Absolute positioning for screens
- CSS transitions: opacity 0.5s cubic-bezier(.4,0,.2,1)
- JavaScript goTo() function for navigation
- Minified CSS for optimization
- Scrollbar hiding on all elements

## No Breaking Changes

- Did NOT add ob-glow or ob-orb elements
- Did NOT change glass-b or glass opacity values
- Did NOT exceed 40px title font-size
- Did NOT use 6px or 8px section labels
- Did NOT make all SVG strokes uniform
- Used only -1px letter-spacing on titles
- Maintained consistent padding/border-radius values

All files are production-ready and use exact design specifications from the accepted NavMap2_Dark.html reference.
