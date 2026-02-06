# Cookie Clicker Access - Features

A comprehensive list of all accessibility features provided by this mod.

## Core Interface

- Big Cookie labeled for screen readers
- Bakery name accessible and focusable
- Cookie count display focusable (tab to check current cookies)
- Cookies per click display below the Big Cookie
- Milk progress display showing current milk type, rank (with Roman numeral), percentage, and achievements until next rank
- Current season display
- News ticker accessible as a heading region, focusable for manual reading
- Options, Statistics, and Info menu buttons labeled and keyboard-accessible
- Legacy/Ascend button with prestige gain information
- FPS counter and undefined elements hidden from screen readers
- Floating number animations hidden from screen readers
- Milk layer visuals hidden from screen readers

## Store and Upgrades

- Store section organized under an H2 heading
- Upgrade shop with full labels showing name, cost, affordability status, effect descriptions, and flavor text
- "Time until affordable" displayed for upgrades that cannot yet be purchased
- Toggle upgrades (Elder Pledge, Elder Covenant, Golden Switch, Shimmering Veil, Season Switcher, Milk Selector, Background Selector) have detailed effect descriptions
- Vaulted upgrades labeled and accessible
- Tech upgrades labeled when visible
- Bulk pricing support (buy/sell 1, 10, 100, or max) with labeled store controls
- Buy/Sell mode toggle buttons labeled and keyboard-accessible

## Buildings

- Available Buildings region with H3 heading
- Building buttons with name, affordability status, cost (including bulk pricing), and count owned
- Building production stats showing cookies per second (individual and total), plus percentage of total CPS
- "Time until affordable" displayed for buildings (adjusts for bulk amount)
- Building info text shown below each building in the store
- Progressive building reveal: owned buildings shown, plus next 1 to buy, plus 1 mystery building (cost only) - matches game behavior
- Building level display with sugar lump upgrade cost and affordability
- Building row labels in the left section with level, minigame status, and upgrade cost
- Level-up buttons labeled with cost in sugar lumps
- Mute buttons labeled per building
- Minigame open/close buttons labeled with correct state

## Minigames

### Garden (Farm)

- Virtual grid navigation system using arrow keys within the 6x6 plot
- "Enter Garden Grid" button to activate arrow key navigation
- Grid coordinates displayed as R#, C# format (e.g., R1, C1)
- Tile information announced: plant name, growth percentage, growth stage (Budding/Growing/Mature)
- Enter/Space to plant selected seed on empty tiles or harvest mature plants
- Home key jumps to R1, C1; End key jumps to last tile
- Escape exits grid navigation
- Garden status display: freeze status, current soil, grid dimensions
- All garden tiles individually labeled with ARIA labels and keyboard support
- Seed selection buttons with plant name, effects, and locked/unlocked status
- Click-to-select announcements when picking seeds
- Soil selector buttons with effects (tick rate, plant effect multiplier, weed multiplier, special effects)
- Soil buttons show locked status with farm requirement
- Garden tools labeled: Information, Harvest All, Freeze/Unfreeze, Sacrifice
- "Harvest Mature Only" button: safely harvests only fully grown plants
- Garden Information panel (collapsible): shows current plant effects and tips
- Section headings for Tools, Soil, Seeds, and Plot areas

### Grimoire (Wizard Tower)

- Magic meter display: current magic, max magic, spells cast, total spells cast
- Each spell organized with H3 heading, cost and status line, effect description, and a Cast button
- Spell cost shows exact magic required and whether you can cast it
- Original spell icons hidden from screen readers (replaced with accessible structure)

### Pantheon (Temple)

- Spirit slots (Diamond, Ruby, Jade) labeled with current occupant or empty status
- Slot buttons on each spirit for quick placement (D, R, J buttons)
- Enter to remove a spirit from its slot
- Spirit headings (H3) with name and current slot status
- Spirit descriptions and buff text accessible as separate focusable elements
- Worship swap count displayed
- Swap cooldown timer shown when no swaps available
- DOM reordering: slots shown first, then spirits in order
- Enhanced Pantheon panel with slot details, effect percentages, and available spirits list
- Active Effects Summary showing current buffs per slot

### Stock Market (Bank)

- Stock rows labeled with name, price, shares owned, and trend (Rising/Falling/Stable)
- Buy, Sell, and Buy Max buttons labeled per stock
- All buttons keyboard-accessible

## Prestige System

- Ascension UI fully accessible
- Heavenly upgrades labeled with name, owned/affordable status, cost in heavenly chips, and description
- Heavenly Chips counter displayed on ascension screen (fixed position, live-updating)
- Permanent upgrade slots (1-5) accessible via keyboard with selection dialog
- Upgrade selection dialog: searchable list with Arrow Up/Down navigation, Enter to select, Escape to cancel
- Reincarnate button labeled and keyboard-accessible

## Special Features

### Dragon (Krumblor)

- Dragon tab labeled as "Krumblor the Dragon"
- Pet Dragon button accessible
- Upgrade Dragon button with current level display
- Dragon Aura slot selection via accessible dialog
- Aura dialog: lists all available auras, Arrow Up/Down navigation, Escape to cancel
- All option buttons within dragon popup keyboard-accessible

### Santa

- Santa tab labeled as "Santa's Progress"
- Pet Santa button accessible
- Upgrade Santa button with current level (out of 14) and max level indicator
- All option buttons keyboard-accessible

### Shimmers (Golden Cookies, Wrath Cookies, Reindeer)

- Live announcements when Golden Cookies, Wrath Cookies, or Reindeer appear
- Seasonal variant names: Golden/Wrath Bunny (Easter), Heart (Valentine's), Pumpkin (Halloween), Contract (Business Day)
- Fading alerts 5 seconds before shimmers disappear
- Active Shimmers panel with clickable buttons showing variant name and countdown timer
- Click announcements showing buff effect when collecting shimmers
- Cookie Chain tracking: announces start and end with total cookies earned
- Cookie Storm tracking: announces start and end with click count
- Rapid-fire event suppression to prevent announcement spam during chains/storms

### Wrinklers

- Wrinkler section with H2 heading
- Spawn announcements (regular and shiny wrinklers)
- Accessible buttons showing cookies sucked per wrinkler
- Click to pop with cookie reward announcement (110% return, 3x for shiny)
- "No wrinklers present" message when none active
- Proper list semantics (role="list" and role="listitem")

### Buffs

- Active Buffs panel with H2 heading
- Each buff displayed with name, remaining time, and effect description
- Buff start announcements with full duration
- Buff end announcements
- "No active buffs" message when none active

### Season Changes

- Notifications when seasons change (start and end)
- Current season display in main interface

### Sugar Lumps

- Sugar lump button labeled with type (Normal, Bifurcated, Golden, Meaty, Caramelized)
- Ripeness status: Growing (time until ripe), Ripe (time until mature), Mature and ready
- Current lump count displayed
- One-time announcement when lump becomes ripe

### Shimmering Veil

- Alert when Shimmering Veil is broken by a Golden Cookie

### Achievements

- Achievement unlock announcements with name and description
- Statistics screen achievements labeled (unlocked: full info; locked: hidden as "???")
- Shadow achievement indicator

### Selectors (Quality of Life)

- Milk Selector labeled (only when unlocked via heavenly upgrade)
- Background Selector labeled (only when unlocked via heavenly upgrade)
- Season Selector labeled (only when Season Switcher upgrade owned)
- Sound/Volume Selector labeled with current status

## Accessibility Infrastructure

- Polite and assertive ARIA live regions for screen reader announcements
- Proper ARIA labels, roles, and tabindex throughout the interface
- Keyboard support (Enter/Space) on all interactive elements
- Structural headings (H2, H3) for screen reader navigation
- Visual elements hidden from screen readers where appropriate
- Debug upgrades hidden from display
- Statistics menu sections labeled as regions with proper headings
- Batch processing for large element sets to avoid UI freezing
