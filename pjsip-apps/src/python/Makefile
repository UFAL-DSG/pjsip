all:
	bash -c "make -s -f helper.mak inc_dir > inc_dir.txt"
	bash -c "make -s -f helper.mak lib_dir > lib_dir.txt"
	bash -c "make -s -f helper.mak libs > libs.txt"
	python setup.py build

clean distclean realclean:
	python setup.py clean
	rm -rf ./build

install:
	python setup.py $@

dep doc:

