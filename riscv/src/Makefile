all:
	riscv64-unknown-elf-gcc -march=rv64g -mabi=lp64 -static -mcmodel=medany   -fvisibility=hidden -nostdlib -nostartfiles -Thello.ld hello.s -o hello

qemu:
	qemu-system-riscv64 -nographic -machine virt -bios none -kernel hello

clean:
	rm hello
