# vim-speeddating

Use `<C-A>`/`<C-X>` to increment dates, times, etc.

Based on [vim-speeddating][1] by Tim Pope, this version adds:

- [ISO 8601][2] date and time formats to the default list
  - `YYYY-MM-DDTHH:MM:SS-0000` - ISO 8601 date & time expressed in UTC
  - `YYYY-MM-DD` - ISO 8601 date
- Alternative default keybindings for updating to the current local or UTC time
  - `z<C-A>` - update **Z**ulu, UTC "military" time
  - `z<C-X>` - update local time **Z**one

## How to use speeddating.vim

Take the following date:

    1999-12-31

Because Vim treats the hyphen as a negative sign, pressing `<C-A>` on the 31
would normally increment it to

    1999-12-30

Compare this with what happens when speeddating.vim is installed:

    2000-01-01

Pressing `5<C-X>` on the `03` in the first line below transforms it into the
second:

    Sat, 01 Jan 2000 00:00:03 +0000
    Fri, 31 Dec 1999 23:59:58 +0000

Several date, time, and datetime formats are included. Additional formats can
be defined in a strftime-like syntax with the `:SpeedDatingFormat` command.

Existing Vim semantics are preserved. `<C-A>` and `<C-X>` accept a count, and
plain number incrementing is used if no date format is matched.

Use of `<C-A>`/`<C-X>` in visual mode enables incrementing several lines at
once. Blank spots are filled by incrementing the match from the previous
line, allowing for creation of sequences (1, 2, 3; 2000-10-30, 2000-10-31,
2000-11-01).

It can also increment roman numerals and ordinals (1st, 2nd, 3rd, ...). In
visual mode, letters of the alphabet are supported.

`z<C-X>` sets the timestamp under the cursor to the current time. `z<C-A>`
does the same, but uses UTC rather than the local time.

The `.` command will work as expected if you install
[repeat.vim](https://github.com/tpope/vim-repeat).

## Contributing

See the contribution guidelines for
[pathogen.vim](https://github.com/tpope/vim-pathogen#readme).

Like speeddating.vim?  Follow the repository on
[GitHub](https://github.com/tpope/vim-speeddating) and vote for it on
[vim.org](http://www.vim.org/scripts/script.php?script_id=2120).

Follow [tpope](http://tpo.pe/):

- [Twitter](http://twitter.com/tpope)
- [GitHub](https://github.com/tpope)

## License
See Copyright © Tim Pope. Distributed under the same terms as Vim itself.
Available at [tpope/vim-speeddating][1]. See `:help license`.

[1]: https://github.com/tpope/vim-speeddating "tpope/vim-speeddating: speeddating.vim: use CTRL-A/CTRL-X to increment dates, times, and more"
[2]: https://en.wikipedia.org/wiki/ISO_8601 "ISO 8601 - Wikipedia"

