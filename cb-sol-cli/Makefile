SOL_URL=https://github.com/hoale58-vl/chainbridge-solidity

fetch-contracts:
	@echo " > \033[32mFetching chainbridge-solidity contracts... \033[0m "
	git clone ${SOL_URL} && cd chainbridge-solidity

compile:
	cd chainbridge-solidity && yarn && npx truffle compile

install: fetch-contracts compile
	@echo " > \033[32mInstalling cb-sol-cli... \033[0m "
	npm link .

clean:
	rm -rf chainbridge-solidity/
