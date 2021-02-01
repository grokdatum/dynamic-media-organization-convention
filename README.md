# dynamic-media-organization-convention

Conventions:
* Filenames should be "normalized", e.g. converted to [a-z0-9] and periods "."
* Based on queries, nested or flat
* Auto-sort by first character, [a-z0-9]
* Directory structure results in a series of nested "repos", I name repos as ...repo.name...
* Anytime a directory listing grows beyond 1 screen of data, do an alphanumeric sort into directories such as ./0.../ through ./9.../ and ./a.../ through ./z.../
** This ensures that no single directory (other than leaf dirs) will grow beyond 36 named entries.
* Files should be tagged like this:
** this.is.a.file...TAG1.TAG2.TAG3...txt
** if you don't like periods then you can use spaces or underscores, I use periods because they are bash friendly and necessary for extensions already.

