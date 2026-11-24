# 1st-Crack-At-It

Bare-metal **Kali Linux** setup running on an external **Samsung Portable SSD T9** (`04e8:61fd`).

## System Setup & Optimizations
- **SSD TRIM:** Enabled `unmap` provisioning over USB via custom `udev` rule (`/etc/udev/rules.d/10-trim.rules`) and `fstrim.timer`.
- **Backups:** Baseline RSYNC system snapshot configured via **Timeshift**.
- **Dotfiles:** Custom `.zshrc` aliases tracked and backed up directly to this repository.

## Custom Aliases
- `update` — Full system upgrade, autoremove, and manual `fstrim`
- `myip` — Display local interfaces and public IP
- `serve` — Start a quick Python HTTP server on port `8000`
- `savekali` — Sync `~/.zshrc` and setup notes straight to GitHub
