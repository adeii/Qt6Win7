# Qt6Win7

--- Test 1 ---
  
Qt 6.5.2 x64 with patches for Qt 6.5.3 x64 for Win 7 (by crystalidea)

Asks for dependancies from Strawberry Perl/C (extras.7z)

Works fine on Win 7/8.x x64.


Built with moz-build :D and portable M$ VS 2017

      git clone https://code.qt.io/qt/qt5.git qt6
      cd qt6
      git switch 6.5.2

      perl init-repository
      ./configure -init-submodules -submodules qtdeclarative

      cd qtbase
      patch  patch -p1 < changes.patch
      cd ..
  

      cmake --build . --parallel 4
      cmake --install .
      
      
--- Test 2 ---

Newest MPC-Qt source with reverting to https://github.com/mpc-qt/mpc-qt/tree/e6177e8b9fd4c8989590c8e84778afcf90188dfb

Compiled with Qt 5.15.1 and minGW81_32bit.

Modded libmpv-2.dll 32bit - demands enabled VxKex (damn!)

Repack of Clementine/Strawberry Music Player is added.


--- Test 3 ---

Qt 6.8.0 x64 compiled as the same as Qt 6.5.3
Got few errors with VxKex.h about reading DPI functions (for Win 10/11). Works fine on Win 7.

--- Test 4 ---

Qt 6.8.1 x64 compiled as the same as Qt 6.5.3, on Win 7, with VS 2022 17.3.
Got fewer modules than 6.8.0. cause low storage space.

--- Test 5 ---

On the way to use Viber 24/25 on Win 7/8, using VxKex and forcing use of OpenGL or Vulkan...

--- Test 6 ---
  
Qt 6.5.3 x64 with patches for Win 7 (by crystalidea), because it is used by few softwares.

--- Test 7 ---
  
Qt 6.10.0 x64 with patches for Win 7 (by ANightly), because it is used by few softwares.

--- Test 8 ---
  
Qt 6.10.2 x64 with fixing patches for Win 7 (by ANightly).
