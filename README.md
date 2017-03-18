# simpleBreakpad-cpp
simple c++ application integrated with the crashrepoting lib google breakpad

# steps :
1 - clone the github repo 

``` $ git clone https://github.com/xMarcoied/simpleBreakpad-cpp ```

2 - build and configure the breakpad library

( This will generate libbreakpad.a and libbreakpad_client.a into the src folder )

``` $ cd simpleBreakpad-cpp ```

``` $ ./configure && make  ```


3 - Linking the generated library with the app.cpp and compile them

``` $ make ```


4 - run the buggy application to generate the minidumps 

``` & make run ```

Now , you can find the dump in the dumps folder .
