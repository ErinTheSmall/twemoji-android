## Building Twemoji

Building Twemoji requires a few files from nototools.  Clone a copy from
https://github.com/googlei18n/nototools and either put it in your PYTHONPATH or
use 'python setup.py develop' ('install' currently won't fully install all the
data used by nototools).  You will also need fontTools, get it from
https://github.com/behdad/fonttools.git.

Then run make.  Twemoji is the default target.  It's suggested to use -j,
especially if you are using zopflipng for compression.  Or you can use `NOCOMPRESSING=1`
to skip compressing.  Intermediate products (compressed image files, for example)
will be put into a build subdirectory; the font will be at the top level.

## License

Tools are under the [Apache license, version 2.0](./LICENSE).

[Twemoji CC-BY 4.0 license](https://creativecommons.org/licenses/by/4.0/)
