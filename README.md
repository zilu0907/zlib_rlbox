# zlib_rlbox

## files:

zpipe.c - the example program provided by zlib (original file)

zpipe_noop.c - sandbox zpipe with no-op sandbox without verification

zpipe_verify.c - sandbox zpipe with no-op sandbox with verification

zpipe_sandbox.c - change no-op sandbox to other sandbox(to do)



## how to run:

1.download zlib onto your computer

2.compile using the following command(depend on your compiler it may work or not work)

c++ -std=c++17 zpipe_xxx.c -lz

3.run the following command to compress:

./a.out < test.txt > test.txt.z

4.run the following command to decompress:

./a.out -d < test.txt.z > test2.txt

## compile with cmake

makedir build
cd build
cmake ..
cmake --build .

