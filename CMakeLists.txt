# Set current dir
CU_SET_PATH("CUR_DIR_MODULE_NOTIFY_MUTED" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/PlayerNotSpeak.cpp")
AC_ADD_SCRIPT_LOADER("PlayerNotSpeak" "${CMAKE_CURRENT_LIST_DIR}/src/loader.h")
CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")
