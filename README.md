# BlockCompressedInt

Using a level-packer on top of a FastPFor decompression of an integer list for optimal memory efficiency. 

Wraps a integer[] in the best known packing algoritm for integers using the FastPFor https://github.com/lemire/FastPFor.
But allow searching in the full structure without decompressing the whole sequence. This is done by block compression and decompressing when
searching. 

Search is very slow, but memory usage will only increase slightly during search because of the level-packer, compared to decompressing the whole int[]

**A very theoric prototype that only makes sense to use if memory is a limited resource and time is not....**



Thomas Egense
