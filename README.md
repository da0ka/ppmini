# ppmini
This program is written in JavaScript + HTML. Its size is smaller than 970bytes! compression raito is usually better than gzip(especially text file).
## f2f-tiny.htm
smallest implementation. Its code is minified. GUI is very simple. and description is too small.
### usage
* o[number] -- input context order. range is 0-255. empty means 0. best balanced value is 2.
* dec -------- if checked it then unpack file else pack file.
* DL --------- if process is done, click here to download file.
## rich.htm
Its GUI is rich. Its code is not minified. But size is over than 3KB.
### usage
* mem[number] --- max count of context model. range is 0-255. Its value is converted to 1e4*number. 0 means unlimited.
* order[number] - It is the same as f2f-tiny.htm of 'o'.
* unpack -------- if checked it then unpack file else pack file.
## ppmini.js
Its file includes a function 'S' only. S does encoding/decoding. no need for above all html.
### usage
S(S,k,d)
* @S ------ Array / Uint8Array.
* @k ------ context order. range is 0-255. empty means 0. best balanced value is 2.
* @d ------ false means encoding. true means decoding
* return -- if @d is false, return packed @S else unpacked @S.
