##[Gh-pages](https://danelsgit.github.io/monorepo-wos-layout-planner/)

# 🗺️ Whiteout Survival - Layout Builder

An enhanced map layout builder for Whiteout Survival game strategy planning.

## 📋 Credits

**Original Author:** [GFXSpeed](https://github.com/GFXSpeed)  


This enhanced version includes additional features for advanced team coordination and strategy planning.[1]

***

## ✨ Features

### Core Features (Original)
- **Interactive Map Builder** - Diamond grid canvas for Castle and Base modes
- **City Management** - Place and label cities with march time calculations
- **Building Placement** - Add flags, obstacles, nodes, and HQ markers
- **Wave Mode** - Visual wave indicators for coordinated attacks
- **Import/Export** - Share layouts via compressed codes
- **High-Quality Export** - Save layouts as PNG images

### 🆕 Enhanced Features (Added)

#### 1. **Enemy Zones** ⚫
- Place up to **3 enemy zones** (12x12 grid size)
- Black zones with "ENEMIES STATE" label
- Castle mode exclusive feature
- Perfect for marking hostile territories

#### 2. **Dynamic Team System** 🎨
- Create **unlimited custom teams**
- Assign custom names (Wave 1, Attackers, etc.)
- Choose any color using hex codes
- Quick assignment via dropdown in Cities section
- Team colors applied to city backgrounds
- Automatic team management and cleanup

#### 3. **Enhanced PNG Export** 💎
- Automatic **2K resolution export** (2x quality)
- No separate button needed
- Perfect for printing and presentations
- High-quality visuals for strategy documentation

#### 4. **Advanced Sorting** 📊
- Sort cities by **Team** (groups by team assignment)
- Sort by **Name** (alphabetical)
- Sort by **BT1/BT2 Time** (march times)
- Combined sorting options
- Default sorting by Team for better organization

***


## 📖 How to Use

### Creating Teams
1. Open **Cities** section in right panel
2. Click **"+ New Team"**
3. Enter team name (e.g., "Wave 1", "Defenders")
4. Enter hex color code (e.g., #3B82F6)
5. Team appears in list with delete option

### Assigning Cities to Teams
1. In Cities section, find your city in the list
2. Use **dropdown menu** next to city name
3. Select team from list
4. City color updates automatically on map
5. Text remains black for readability

### Placing Enemy Zones
1. Switch to **Castle mode**
2. Click **"Enemy Zone"** button
3. Click on map to place (12x12 size)
4. Maximum 3 zones allowed
5. Delete with Select tool + Delete key

### Exporting Layouts
- Click **"Save as PNG"** - automatically exports in 2K quality
- Use **"Get Code"** to share layout via compressed string
- Layouts save team assignments automatically

***

## 🎨 Team Color System

**How It Works:**
- City background = Team color
- No team assigned = Random/original color
- Visual grouping on map by color

**Example Use Cases:**
- **Attack Waves:** Wave 1 (Red), Wave 2 (Blue), Wave 3 (Green)
- **Roles:** Attackers (Orange), Defenders (Purple), Support (Yellow)
- **Players:** John's targets (Pink), Mike's targets (Cyan)

***

## ⚙️ Technical Details

### New Variables
- `enemyZones[]` - Array of enemy zone entities
- `cityTeams{}` - City-to-team assignments
- `customTeams[]` - Dynamic team list with names and colors

### New Functions
- `initializeDefaultTeams()` - Initialize with 1 default team
- `createNewTeam()` - Team creation dialog
- `deleteTeam(index)` - Remove team and cleanup assignments
- `assignCityToTeam()` - Assign/unassign cities
- `updateTeamsUI()` - Refresh team list display
- `drawEnemyZoneDetails()` - Render enemy zones

### Modified Functions
- `drawEntity()` - Apply team colors to cities
- `drawCityDetails()` - Keep text black
- `updateCityList()` - Add team dropdowns and sorting
- `enablePopulateSortOptions()` - Team/Name sort options
- `downloadCanvasAsPNG()` - 4K export automatically

***


## 📄 License

Please refer to the original repository for licensing information.

## 🙏 Acknowledgments

**Special thanks to [GFXSpeed](https://github.com/GFXSpeed)** for creating the original Layout Builder that made these enhancements possible.

***

**Enjoy strategic planning with enhanced team coordination features!** 🎯
