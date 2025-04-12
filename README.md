# Cryptor
Tinkering with data compression and encryption

Cryptor is a fast (as in gzip fast) arithmetic coder with similar or better level of compression to that tool.

The arithmetic coder part is a C# implementation of the coder described in Barry Stratford's 2005 paper (see included pdfs and his reference code in separate folder)

Cryptor has 2 levels of compression:
1. A simple, very fast, adaptive model (relatively low compression -- compressing catenated calgary corpus to ~55%, and enwiki8 to ~62%)
2. A novel adaptive model (in the PPM family) that compresses at the same level, or slightly better, than gzip, with similar performance.
   (It compresses the catenated calgary corpus to ~34%, and enwiki8 to ~32%)

The encoder also includes almost zero-cost strong encryption through a key and/or iv.


