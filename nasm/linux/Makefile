hello: hello.o
	ld -no-pie -e main -o $@ $<

hello.o: hello.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

printf: printf.o
	gcc -o $@ $< -no-pie

printf.o: printf.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

function: function.o
	gcc -o $@ $< -no-pie

function.o: function.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

func-args: func-args.o
	gcc -o $@ $< -no-pie

func-args.o: func-args.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

simd-intro: simd-intro.o
	gcc -o $@ $< -no-pie

simd-intro.o: simd-intro.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

align: align.o
	gcc -o $@ $< -no-pie

align.o: align.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

half-adder: half-adder.o
	gcc -o $@ $< -no-pie

half-adder.o: half-adder.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

jnz: jnz.o
	gcc -o $@ $< -no-pie

jnz.o: jnz.asm
	nasm -f elf64 -g -F dwarf -o $@ $<

clean:
	$(info "cleaning...")
	rm -rf hello printf function

