all:

clean:
	rm -f *~ *.bin *.bin.hex *.gz *.addr *.zip

play_on_sandbox:
	./00_init_sandbox.sh
	$(MAKE) play_tests

play_on_testnet:
	./00_init_testnet.sh
	$(MAKE) play_tests

play_tests:
	./01_prepare.sh
	./02_deploy.sh
	./03_solve_sudoku.sh
	./04_new_instance.sh
	./05_get.sh
	./06_submit_false_solution.sh
	./07_submit_false_proof.sh
