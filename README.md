# ppmini
This program is written in JavaScript + HTML. Its size is smaller than 970bytes! compression raito is usually better than gzip.
## f2f-tiny.htm
smallest implementation. Its code is minified. GUI is very simple. and description is too small.
### usage
* o[number] -- input context order. range is 0-255. empty means 0. best balanced value is 2.
* dec -------- if checked it then unpack file else pack file.

## rich.htm
Its GUI is rich. Its code is not minified. But size is over than 3KB.
### usage
* mem[number] --- max count of context model. range is 0-255. Its value is converted to 1e4*number. 0 means unlimited.
* order[number] - It is the same as f2f-tiny.htm of 'o'.
* unpack -------- if checked it then unpack file else pack file.
