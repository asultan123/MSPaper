TARGET := ../fig/
PDF := $(patsubst %.drawio,%.pdf,$(addprefix $(TARGET),$(wildcard *.drawio)))
all: $(PDF)
	$(info All figures compiled)

$(TARGET)%.pdf: %.drawio
	$(info Compiling $(*))
	drawio --export -t --width 1024 -f pdf -o $(TARGET)$*.pdf $*.drawio
