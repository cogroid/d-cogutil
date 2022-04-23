ROOT_DIR=../../

all: src_update lib_copy

src_update:
	cp -f ${ROOT_DIR}/make/i386/OpenCogGccOptions.cmake ${ROOT_DIR}/cmake/

lib_copy:
	sudo mkdir -p /home/cogroid/local/lib/i386
	sudo cp -rf ${ROOT_DIR}/make/i386/lib/* /home/cogroid/local/lib/i386/

clean: uninstall
	cp -f ${ROOT_DIR}/make/i386/org/OpenCogGccOptions.cmake ${ROOT_DIR}/cmake/

uninstall:
	sudo cp -f /home/cogroid/local/lib/i386.org/libcogutil.so /usr/local/lib/opencog/

install:
	sudo mkdir -p /home/cogroid/local/lib/i386.org
	sudo mkdir -p /usr/local/lib/opencog
	sudo cp -f /usr/local/lib/libcogutil.so /home/cogroid/local/lib/i386.org/
	sudo cp -f ${ROOT_DIR}/build/opencog/util/libcogutil.so /usr/local/lib/opencog/
