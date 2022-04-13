# Makefile to create an environment from the command line

# This target creates an environment first, and then configures it by 
# activating it and installing ipykernel into it.  Note that for the 
# activation/install commands to work, they must be executed in a single
# line that is prefixed with `bash -ic` - this executes them under an 
# interactive shell, which is required for `conda activate` to work.

.PHONY: env
env:
	mamba env create -f environment.yml
	bash -ic 'conda activate ligo;python -m ipykernel install --user --name ligo --display-name "IPython - ligo"'
