SUBDIR =  \
		  component\
		  net\
		  process\

all: targets

targets:
	@for subdir in $(SUBDIR); do  \
		$(MAKE) -C $$subdir || exit 1 ; \
		done 

clean:
	@for subdir in $(SUBDIR); do  \
		(cd $$subdir && $(MAKE) clean); \
		done

distclean:
	@for subdir in $(SUBDIR); do  \
		(cd $$subdir && $(MAKE) distclean); \
		done

ctags:
	ctags -R
