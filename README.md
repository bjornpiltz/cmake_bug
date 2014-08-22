cmake_bug
=========

A project which shows a problem with the scope of imported libraries.

With cmake 3.0.1 the following

    git clone https://github.com/bjornpiltz/cmake_bug.git cmake_bug
    mkdir work
    cd work
    cmake -DCMAKE_PREFIX_PATH=<Qt5>/lib/cmake/ ../cmake_bug/

produces:

    -- Configuring done
    CMake Error at CMakeLists.txt:5 (add_executable):
      Target "app" links to target "Qt5::Core" but the target was not found.
      Perhaps a find_package() call is missing for an IMPORTED target, or an
      ALIAS target is missing?
