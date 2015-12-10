This is the source code of the original Unix 'spell' program, as described in McIlroy (1982). The source code was extracted from original Unix archives from 1978-1981. All modern spell-checker programs (ispell/aspell/pspell etc) are descendants of this source code.

[McIlroy 'spell' paper (1982) (pdf)](http://unix-spell.googlecode.com/svn/trunk/McIlroy_spell_1982.pdf)

The paper describes two methods:
  * Method 1 - **bloom filter** - source code and dictionary: [/method1](http://code.google.com/p/unix-spell/source/browse/#svn/trunk/method1)
  * Method 2 - **differential Huffman coded hash** - source code and dictionary: [/method2](http://code.google.com/p/unix-spell/source/browse/#svn/trunk/method2)

The whole thing: [spell\_r4.zip](http://unix-spell.googlecode.com/files/spell_r4.zip)

It is interesting to note that one of the world's best compressor (paq8l) can compress the 250kb word list down to 48.5kb, less than the space taken by the lossy compression methods proposed in the paper! For comparison, regular modern compression methods (such as gzip, lzma etc) only achieve twice that size (85-90kb).

Happy hacking!

Larry (lrrdavis0@gmail.com)