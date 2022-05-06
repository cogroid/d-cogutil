all:
	sudo mkdir -p /home/cogroid/local/d-cogutil/x64
	mkdir -p ../../build
	cd ../../build; \
	cmake \
	-DCMAKE_INSTALL_PREFIX="/home/cogroid/local/d-cogutil/x64" \
	..; \
	make

install:
	sudo sh -c 'cd ../../build; \
	make install;'

clean:
	rm -rf ../../build