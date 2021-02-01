# dynamic-media-organization-convention

Conventions:
* These conventions allow for media helper scripts, such as sorting subdirectories by first character, or converting directory structures from flat to nested.
* Filenames should be "normalized", e.g. converted to [a-z0-9] and periods "."
* Filename should embed a hash such as SHA256, you can truncate it to 16 or so Characters, example "this.is.a.file...ABCDEF1234567890...txt.
* This helps with tasks like de-duplication and bit-rot detection.
* Based on queries, nested or flat
* Auto-sort by first character, [a-z0-9]
* Directory structure results in a series of nested "repos", I name repos as ...repo.name...
* Anytime a directory listing grows beyond 1 screen of data, do an alphanumeric sort into directories such as ./0.../ through ./9.../ and ./a.../ through ./z.../
  * This ensures that no single directory (other than leaf dirs) will grow beyond 36 named entries.
  * Subdirectories under dirs like ./a.../ can either be nested or flat, such as ./a.../a/few/good/men/ or ./a.../a.few.good.men.../, use the former if you have too many entries under ./a.../ or the latter if you have less than a screen full of subdirectories.
* Files should be tagged like this:
  * this.is.a.file...TAG1.TAG2.TAG3...txt
    * These tags should be part of a controlled vocabulary of userdefined tags, Tags can mean anything, such as preferred media, genre (Ebooks), Source (YOUTUBE), etc.
  * if you don't like periods then you can use spaces or underscores, I use periods because they are bash friendly and necessary for extensions already.
* repo names can be based on just about anything, examples include:
  * subject of video (e.g. rihanna)
  * producer of media (e.g. Ebook producer)
  * genre of media
  * audience of media (family / friends / public / private / etc)
  * preference of media (favorites, expendable, etc.)
  * HD / 4K / 4K+ Video.
  * author of content.
  * method or engine of collection (youtube-dl, gallery-dl, wget, etc)
  
  These conventions should result in a very nested collection of directories such as the following:


```

./datahoard/.../0.../
./datahoard/.../a.../
./datahoard/.../b.../

```
