# mussort - a Simple music file sorting program

`mussort` recursively searches a directory for MP3, OGG Vorbis and FLAC files, processing them one by one. It then reads the information from the file and puts them into a newly sorted directory tree.

## Dependencies

- `Try::Tiny` (perl module)
- For OGG vorbis support, one or more of: `Ogg::Vorbis::Header::PurePerl` (perl module), `Ogg::Vorbis::Header` (perl module), `Audio::File` (perl module) or `ogginfo`
- For MP3 (ID3) support, one or more of: `id3v2`, `id3info`, `Audio::File` (perl module)
- For FLAC support, one or more of: `metaflac`, `Audio::File` (perl module)
- Additionally, as it is written in perl, perl is required.

When installing from the git repository, the `pod2man` utility is required to
create the manpage (not needed in release tarballs as those already include the
generated manpage).

## Installation

To install it as a user run `make install`. To install as root run the same command as root. To "install" a working copy (ie. a git checkout) use `make localinstall`, this will just set up symlinks that point to the mussort command and manpage, allowing your copy in PATH to be up-to-date while working.

## License

Copyright © Eskild Hustvedt 2007-2016

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program. If not, see http://www.gnu.org/licenses/.
