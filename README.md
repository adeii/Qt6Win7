# Qt6Win7

* Test 1 *
Qt 6.5.2 x64 with patches for Qt 6.5.3 x64 for Win 7 (by crystalidea)

Asks for dependancies from Strawberry Perl/C (extras.7z)

Works fine on Wi 8.x x64.


Build with moz-build :D and portable M$ VS 2017

      git clone https://code.qt.io/qt/qt5.git qt6
      cd qt6
      git switch 6.5.2

      cd qtbase
      patch  patch -p1 < changes.patch
      cd ..
  
      perl init-repository
      ./configure -init-submodules -submodules qtdeclarative
      cmake --build . --parallel 4
      cmake --install .
      
      
