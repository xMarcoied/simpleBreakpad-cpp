# simpleBreakpad-cpp
simple c++ application integrated with the crashrepoting lib google breakpad

(check the wiki [https://github.com/xMarcoied/simpleBreakpad-cpp/wiki] for more details about the project.)
# steps :
1 - clone the github repo 

``` $ git clone https://github.com/xMarcoied/simpleBreakpad-cpp ```

``` $ cd simpleBreakpad-cpp ```

2-a - downloading the breakpad library

``` $ git clone https://chromium.googlesource.com/breakpad/breakpad ```


2-b - build and configure the breakpad library

( This will generate libbreakpad.a and libbreakpad_client.a into the src folder )

``` $ cd breakpad ```

``` $ ./configure && make  ```


3 - Linking the generated library with the app.cpp and compile them
``` $ cd ..  ```

``` $ make ```


4 - run the buggy application to generate the minidumps 

``` $ make run ```

Now , you can find the dump in the dumps folder .
