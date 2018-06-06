rustaceans.org
==============

[rustaceans.org](http://www.rustaceans.org) is a website for finding information
about members of the Rust community. This repository contains details of
rustaceans and provides the data for rustaceans.org. To see the source itself
for rustaceans.org, see https://github.com/nick29581/rustaceans-src.

To add or edit your data, you must fork this repo and send a pull request. Your
PR should only add/modify a single file named `<your github username>.json` in
the `data` directory. If your PR touches only your file, it will be
automatically merged and the database for rustaceans.org is automatically
updated.

To remove yourself from rustaceans.org, send a PR removing your json file. Note
that your data will remain in the public history of this repository and cannot
be removed.

[data/template.json](https://github.com/nick29581/rustaceans.org/blob/master/data/template.json)
is a template json file you can fill in with your details. Make sure you don't
delete the original file or your PR will be rejected. All fields are optional
(but your GitHub username will always be shown on rustaceans.org). You can add
any fields you like; they will be ignored, but if that field is added to
rustaceans.org in the future it will get picked up. Feel free to obfuscate any
fields you like (such as `email`).

### The fields

* `name` - Your name.
* `email` - Your email address. Will appear in a mailto link.
* `website` - Your homepage URL.
* `blog` - URL for your blog.
* `irc` - Your IRC nickname.  (Does not support different nicknames for
  different servers; use the nickname you use on Rust IRC channels.)
* `irc_channels` - a json array of channel names on `irc.mozilla.org`, without
  the `#` (e.g. `["rust", "rust-gamedev"]`).
* `discourse` - Your username on [Discourse](https://internals.rust-lang.org/).
* `reddit` - Your username on [Reddit](https://www.reddit.com/r/rust/)
* `twitter` - Your username on [Twitter](https://twitter.com/), including the
  `@`.
* `patreon` - Your username on [Patreon](https://www.patreon.com/)
* `show_avatar` - `true` or `false`, if it is true, your GitHub avatar will be
  displayed on rustaceans.org
* `notes` - any notes you like about yourself. Markdown format; make sure you
  escape newlines and double quotes.

## License and copyright

Each file in this repository is copyright (2014) that file's author. By
submitting a file to this repository, you give permission for the contained data
to be stored and displayed on rustaceans.org. This permission may be withdrawn
at any time by sending a pull request removing the file and the data will be
removed from rustaceans.org within a reasonable time. No files in this
repository may be copied, modified, or distributed for commercial use.
