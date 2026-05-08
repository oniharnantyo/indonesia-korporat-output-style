# Indonesia Korporat Output Style

Punten, ini adalah Claude Code plugin yang automatically applies authentic Indonesian corporate communication style ke semua respons Claude. Perfect untuk professionals yang working di Indonesian corporate environments.

## Quickstart

Ijin kasih quickstart setup buat Indonesian corporate communication style:

```bash
/plugin install https://github.com/oniharnantyo/indonesia-korporat-output-style
```

## How It Works

Punten, plugin ini menggunakan **SessionStart hook** buat automatically inject Indonesian corporate communication style instructions di awal setiap Claude Code session.

Jadi instead of harus remember buat minta Indonesian corporate style, Claude otomatis:

- **Detects formality context** - Adjusts language based on who you're addressing (seniors, team, close teammates)
- **Applies mixed language style** - Uses Indonesian sentence structure dengan English corporate terms (ASAP, PIC, sync up, deadline, alignment, etc.)
- **Uses appropriate politeness markers** - Punten, Izin, Monggo, Mohon arahan based on the situation
- **Integrates naturally** - Terms are used where they fit, not forced

Style-nya applied consistently throughout the entire session tanpa manual activation. Just start Claude dan communicate naturally dalam Indonesian corporate style.

## Installation

### Option 1: Install from GitHub (Recommended)

Ijin install langsung dari GitHub menggunakan Claude Code plugin command:

```bash
/plugin install https://github.com/oniharnantyo/indonesia-korporat-output-style
```

### Option 2: Clone and Install Locally

```bash
# Clone the repository
git clone https://github.com/oniharnantyo/indonesia-korporat-output-style.git

# Install the plugin
cd indonesia-korporat-output-style
claude plugin install
```

### Option 3: Manual Installation

```bash
# Clone atau download the plugin
git clone https://github.com/oniharnantyo/indonesia-korporat-output-style.git

# Navigate ke your project directory
cd /your/project

# Create symbolic link ke plugin
ln -s /path/to/indonesia-korporat-output-style .claude-plugin

# Atau copy plugin directory
cp -r /path/to/indonesia-korporat-output-style .claude-plugin
```

### Option 4: Global Installation

```bash
# Copy ke global plugins directory
cp -r /path/to/indonesia-korporat-output-style ~/.claude/plugins/indonesia-korporat-output-style
```

### Option 5: Using Plugin Directory Flag

```bash
# Start Claude Code dengan plugin directory
claude --plugin-dir /path/to/indonesia-korporat-output-style
```

## Verify Installation

Punten, setelah installation, verify the plugin is loaded:

```bash
/plugin list
```

You should see `indonesia-korporat-output-style` di list of installed plugins.

## The Basic Style

Ijin jelaskan bahwa plugin ini automatically applies Indonesian corporate communication style across three formality levels:

1. **Formal** - Untuk seniors, clients, official meetings
   - Full sentences dengan proper structure
   - Politeness markers (Punten, Mohon arahan, Izin)
   - Deferential tone

2. **Semi-Formal** - Untuk team coordination, project discussions
   - Mixed politeness (respectful tapi less rigid)
   - Common abbreviations (FU, PIC, ASAP, FYI)
   - Collaborative language

3. **Casual** - Untuk close teammates, informal discussions
   - Relaxed politeness (monggo, yuk)
   - Slang terms (low battery mode, burnout, wrap up)
   - Conversational tone

FYI, Claude automatically detects the appropriate formality level based on conversation context dan applies the style consistently.

## What's Inside

### Components

**SessionStart Hook**
- Automatically activates Indonesian corporate communication style di session start
- No manual commands ato configuration needed
- Applies consistently throughout the entire session
- **13,407 characters** of comprehensive Indonesian corporate style content

**Comprehensive Style Content (in Hook Script)**
- Core principles dan MANDATORY rules
- Polite openers & markers (Punten, Ijin, Monggo, Mohon arahan)
- Complete vocabulary reference (27+ terms across categories)
- Detailed formality levels (Formal, Semi-Formal, Casual)
- Communication patterns by scenario (6 scenarios)
- Hierarchy & address guidelines
- Key usage rules
- Common phrases by frequency
- 10 real conversation examples
- Polite closing dengan 🙏 emoji guidance

### Common Vocabulary

**Discussion & Meeting**: Jump in, Alignment, Sync up, Circle back, Wrap up, Deep dive, Parking lot

**Task & Execution**: Follow up (FU), Actionable items, PIC, ASAP, Deadline (Soft/Hard), Deliverables

**Response & Feedback**: Noted / Well noted, Please kindly check, Feedback, FYI, CC / BCC

**Status & Condition**: Low battery mode, Burnout, Hustle culture, Work-life balance, Adjust

**Polite Markers**: Punten, Izin, Monggo, Mohon arahan

## Philosophy

Punten, Indonesian workplace culture values:

- **Harmony** dalam communication
- **Respect untuk hierarchy** (seniors, superiors, clients)
- **Indirect communication** untuk sensitive topics
- **Collaborative language** dalam team settings

Plugin ini captures those cultural nuances sambil maintaining efficiency dari modern corporate communication. The goal adalah **natural Indonesian corporate communication**, bukan caricature.

## Example Interactions

**Formal (Reporting ke Superior):**

```
User: How do I report project progress?

Claude: Punten Pak/Bu, untuk melaporkan progres proyek, bisa melalui email
atau meeting standup. Mohon arahan format laporan yang diharapkan.
```

**Semi-Formal (Team Coordination):**

```
User: Remind the team about the deadline

Claude: Oke tim, FYI deadline untuk deliverables minggu ini adalah hari
Jumat. Tolong masing-masing PIC sinkronisasi progres dan report kalau ada
blocking issue.
```

**Casual (Close Teammate):**

```
User: I'm tired from all these meetings

Claude: Duh, low battery mode banget ya. Yuk wrap up lebih cepat, jangan
lupa jaga work-life balance!
```

## Managing the Plugin

### Enable the Plugin

```bash
/plugin enable indonesia-korporat-output-style
```

### Disable the Plugin

```bash
/plugin disable indonesia-korporat-output-style
```

### Uninstall the Plugin

```bash
/plugin uninstall indonesia-korporat-output-style
```

### Update the Plugin

```bash
/plugin update indonesia-korporat-output-style
```

### Check Plugin Status

```bash
/plugin list
```

## Contributing

Punten, contributions are welcome! Please kindly submit issues ato pull requests untuk improve the plugin.

1. Fork the repository
2. Create a branch untuk your work
3. Make your changes
4. Submit a PR dengan clear description dari changes

## Plugin Structure

```
indonesia-korporat-output-style/
├── .claude-plugin/
│   └── plugin.json          # Plugin manifest
├── hooks/
│   └── hooks.json           # Hook configuration
├── hooks-handlers/
│   └── session-start.sh     # Hook script (13,407 chars of style content)
├── README.md                # This file
├── LICENSE                  # MIT License
└── .gitignore              # Git ignore rules
```

## License

MIT License - See LICENSE file untuk details

## Author

Created oleh [Oni Harnantyo](https://github.com/oniharnantyo)

## Acknowledgments

Ijin sampaikan terima kasih kepada [learning-output-style](https://github.com/anthropics/claude-code/tree/main/plugins/learning-output-style) dan [explanatory-output-style](https://github.com/anthropics/claude-code/tree/main/plugins/explanatory-output-style) plugins untuk SessionStart hook pattern-nya.
