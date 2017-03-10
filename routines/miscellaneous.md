### Buffer objects

getbuffer(obj [,offset[, size]])	Create a buffer object from the given object referencing a slice of length size starting at offset.
newbuffer(size)		Return a new uninitialized buffer object.

### Performance tuning

alterdot()	Change dot, vdot, and inner to use accelerated BLAS functions.
restoredot()	Restore dot, vdot, and innerproduct to the default non-BLAS implementations.
setbufsize(size)	Set the size of the buffer used in ufuncs.
getbufsize()	Return the size of the buffer used in ufuncs.

### Memory ranges

shares_memory(a, b[, max_work])	Determine if two arrays share memory
may_share_memory(a, b[, max_work])	Determine if two arrays might share memory

### NumPy version comparison

lib.NumpyVersion(vstring)	Parse and compare numpy version strings.

