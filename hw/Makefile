decode.jed: decode.pld

%.jed: %.pld
	galasm $<
#	cat $@ | ./fixjed >fixed.jed
#	mv fixed.jed $@

.PHONY: program
program: glue.jed
	minipro -p ATF16V8B -c config -w $<
