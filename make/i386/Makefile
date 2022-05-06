all:
	sudo mkdir -p /home/cogroid/local/d-cogutil/i386
	sudo mkdir -p /home/cogroid/local/d-cogutil/i386/lib
	sudo cp -rf ./lib/* /home/cogroid/local/d-cogutil/i386/lib/
	cp -f ./OpenCogGccOptions.cmake ../../cmake/
	mkdir -p ../../build
	cd ../../build; \
	cmake \
	-DCMAKE_INSTALL_PREFIX="/home/cogroid/local/d-cogutil/i386" \
	..; \
	make

install:
	sudo sh -c 'cd ../../build; \
	make install;'

clean:
	rm -rf ../../build