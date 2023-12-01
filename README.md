# ppmini
This program is file (de)compresseor written in JavaScript + HTML. Its size is smaller than 900bytes! compression raito is usually better than gzip(especially text file).
## f2f-tiny.htm
smallest implementation. Its code is minified. GUI is very simple. and description is too small.
### usage
* o[number] -- input context order. range is 0-255. empty means 0. best balanced value is 2.
* dec -------- if checked it then unpack file else pack file.
* DL --------- if process is done, click here to download file.
## f2f-tiny2.htm
almost the same as f2f-tiny.htm. it uses carryless range coder.
## rich.htm
Its GUI is rich. Its code is not minified. But size is over than 3KB.
### usage
* mem[number] --- max count of context model. range is 0-255. Its value is converted to 1e4*number. 0 means unlimited.
* order[number] - It is the same as f2f-tiny.htm of 'o'.
* unpack -------- if checked it then unpack file else pack file.
## 10items.htm
Included improved versions(Information Inheritance, Secondary Escape Estimation). It outputs program code and its demo. You can download programs from bottom button. usage is the almost the same as f2f-tiny.htm.
Difference is maximum order. program No8 and No10 is 31, others are 7.

## ppmini.js
Its file includes a function 'S' only. S does encoding/decoding. its size is 699bytes. no need for above all html.
### usage
_(k,n,f)
* @k ------ Array / Uint8Array.
* @n ------ context order. range is 0-7. Not a number means 0. best balanced value is 2.
* @f ------ false means encoding. true means decoding
* return -- if @d is false, return packed @S else unpacked @S.
