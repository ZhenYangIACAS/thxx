
all: rapidjson catch.hpp

rapidjson:
	wget -O- https://github.com/Tencent/rapidjson/archive/v1.1.0.tar.gz | tar zxvf -
	ln -s `pwd`/rapidjson-1.1.0/include/rapidjson rapidjson

catch.hpp:
	wget https://raw.githubusercontent.com/catchorg/Catch2/master/single_include/catch2/catch.hpp

libtorch-shared-with-deps-latest.zip:
	wget https://download.pytorch.org/libtorch/cpu/libtorch-shared-with-deps-latest.zip
	unzip libtorch-shared-with-deps-latest.zip

Release_1_8_15.tar.gz:
	wget https://github.com/doxygen/doxygen/archive/$@
	tar -xf $@

doxgen:
	cd ./doxygen*/; mkdir -p build; cd build; cmake .. ; make DESTDIR=stage install

