# vim-speeddating

Use `<C-A>`/`<C-X>` to increment dates, times, etc.

Based on [vim-speeddating][1] by Tim Pope, this version adds:

- [ISO 8601][2] date and time formats to the default list
  - `YYYY-MM-DDTHH:MM:SS-0000` - ISO 8601 date & time expressed in UTC
  - `YYYY-MM-DD` - ISO 8601 date
- Alternative default keybindings for updating to the current local or UTC time
  - `z<C-A>` - update **Z**ulu, UTC "military" time
  - `z<C-X>` - update local time **Z**one

## License
See Copyright © Tim Pope. Distributed under the same terms as Vim itself. See :help license.
Available at [tpope/vim-speeddating][1]

[1]: https://github.com/tpope/vim-speeddating "tpope/vim-speeddating: speeddating.vim: use CTRL-A/CTRL-X to increment dates, times, and more"
[2]: https://en.wikipedia.org/wiki/ISO_8601 "ISO 8601 - Wikipedia"
