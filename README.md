# ssgs

ssgs - A simple static blog generator written in POSIX `sh`.

## Dependencies

* `sh`, `bash`, `zsh` or other shell like UNIX.
* GNU Coreutils, BusyBox, Toybox, sbase or other UNIX utilities.
* [smu - a Simple Markup Language.](https://github.com/karlb/smu)

## Usage

```bash
$ mkdir myblog
$ cd myblog
$ ssgs -b
$ cat << EOF > src/about.md
# About me

Hi everyone!
EOF
$ ssgs -b
```

## Workflow

```text
[myblog]
 ├─[build]
 ├─[src]
 └─ssgs.config
```

* `build` - Contain your HTML blog after executing `ssgs -b`
* `src` - Write your `Markdown` articles in this directory with `*.md` extension, supports subdirectories, images, videos, audios and other files.
* `ssgs.config` - Contain config vars for your blog, see `ssgs.config.def` file.

## Thanks

* [ssg6 - Static site generator written in shell.](https://www.romanzolotarev.com/ssg.html)
* [Dylan Araps - Pure sh bible.](https://github.com/dylanaraps/pure-sh-bible)
* [sw - Suckless web framework.](https://github.com/jroimartin/sw)
* [bashblog - A single Bash script to create blogs.](https://github.com/cfenollosa/bashblog)

## License

```text
ssgs - A simple static blog generator written in POSIX sh.

Copyright (C) 2021-2022 - Ricardo García Jiménez <ricardogj08@riseup.net>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this software except in compliance with the License.
You may obtain a copy of the License at:

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
