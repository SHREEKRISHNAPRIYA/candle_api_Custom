# candle_api for Windows (optional Echo)

-in this i have tried to make a custom binder for the candle library python

## steps to create a binder

-downdoal the candle api with the submodules like cmake,pybind11 ,libusb-1.0.30-rc2 https://github.com/libusb/libusb/releases/download/v1.0.30-rc2/libusb-1.0.30-rc2.7z\
-download zip and pase the lib.h from the ..ibusb-1.0.30-rc2\include to \
..\candle_api_Custom\candle_api\include \

(if not present \
download https://github.com/libusb/libusb-cmake/archive/refs/heads/master.zip \
and paste it in \
candle_api_Custom-main/\
└── candle_api/\
 └── libusb-cmake/\
 ├── CMakeLists.txt ✅ must exist here\

and download https://github.com/pybind/pybind11/archive/refs/heads/master.zip \
and paste it in the \
candle_api_Custom-main/\
└── candle_api_pybind11/\
 └── pybind11/\
 ├── CMakeLists.txt ✅ must exist here with out the outer folder when extracted)\

-download the VS 17 2022 version build tools https://my.visualstudio.com/Downloads?q=visual%20studio%202022&wt.mc_id=o~msft~vscom~older-downloads \
-have following \
REQUIRED\
1.MSVC v143 - VS 2022 C++ x64/x86 build tools\
2.Windows 10 or 11 SDK\
3.C++ CMake tools for Windows\
4.MSBuild\

-open x64 Native command prompt for VS 2022\
-go to the downloaded candle api foalder using cd\
-python setup.py build_ext --inplace (this will give the bindings after build )\
-paste the binder in the C:\...\Python\Python310\Lib\site-packages\candle_api\

-make cahnges and build again if required
