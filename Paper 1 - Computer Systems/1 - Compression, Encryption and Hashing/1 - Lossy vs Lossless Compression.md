
- The purpose of compression is to:
	- Reduce the size of files.
	- Reduce download times.
	- Reduce storage requirements.
	- Make best use of bandwidth.

> The last point works, as by reducing a file's size as much as possible, it takes up a lot less time to transmit.

## Lossy Compression 

- Lossy Compression is a method of compression where the file loses some of its data.
- With Images and videos, this loss of data can be quite significant, and not be very noticeable, which makes it a good choice for this media.

## Lossless Compression

- Lossless Compression is a method where the file loses no data, and is fully recoverable.
- This is done in images by rather than storing every pixel with its binary pattern, it makes patterns of multiple colours in a row.
	- E.g. Rather than white, white, blue, yellow being stored separately as colours, you can store that specific pattern with its own binary code, which would save space.
	- This method only really works for vector drawings, rather than bitmap images, as there is so much complexity in those images that the number of unique patterns would not make much of a difference than the original size of the file.
- Text files can only undergo Lossless, as we need to keep all the data that is stored in the file, as any loss may make it unreadable.


