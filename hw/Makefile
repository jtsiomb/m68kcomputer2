galdev = -p ATF16V8B

.PHONY: all
all: decode.jed iodecode.jed glue.jed

decode.jed: decode.pld

glue.jed: glue.pld

%.jed: %.pld
	galasm $<
#	cat $@ | ./fixjed >fixed.jed
#	mv fixed.jed $@

.PHONY: program-decode
program-decode: decode.jed
	minipro -p ATF16V8B -c config -w $<

.PHONY: program-glue
program-glue: glue.jed
	minipro -p ATF16V8B -c config -w $<

.PHONY: program-iodecode
iodecode-glue: iodecode.jed
	minipro -p ATF20V8B -c config -w $<

.PHONY: clean
clean:
	rm -f *.jed
