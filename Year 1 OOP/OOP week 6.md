### Files

#### Stream handling classes
java doesn't have meaning to a file's content. 
Stream is an object to perform actions, opening, closing, reading, writing 
Most streams flow in one direction
input
has next - checks for more data 
next - gives the next piece of data
Output
write = outputs a data element on the stream

InputStream/OutputStream - reads bytes
Reader/Writer - reading and writing characters 
Scanner, PrintWriter, PrintStream: - reading or writing strings
DataInputStream/ DataOutputStream - reading or writing data values
ObjectInputStream/ ObjectOutputStream- reading or writing data values 
These classes need to implement serializable interface.

Buffers read/write everything to a buffer - temporary storage - before writing to or reading from the file
####  File buffers
using only input and output streams are slow as they read in a byte at a time


#### Random Access files
