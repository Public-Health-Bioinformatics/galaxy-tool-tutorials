# galaxy-tool-tutorials
 Galaxy tool training materials being developed for in-house workshops.

**Galaxy Tool Development**: Overview of how to develop a Galaxy tool wrapper around an existing command line application.  Discusses how to prepare a tool for uploading to a Galaxy shared tool library (toolshed).  Covers basic use of planemo (https://planemo.readthedocs.org/en/latest/) for easier testing.  Assumes an existing Galaxy install server (which has gedit and firefox or other X-windows compatible browser) where tools will be developed.  Also assumes user familiarity with linux command line.

Planemo setup for example:

planemo tool_init --force \
	--id 'blast_comparison' \
	--name 'Blast report comparison' \
	--example_command 'main.py -o dataset_dec_11_2013.tab -n dataset_aug_22_2014.tab -s dataset_log.txt' \
	--example_input dataset_dec_11_2013.tab \
	--example_input dataset_aug_22_2014.tab \
	--example_output dataset_log.txt \
	--test_case \
	--help_from_command 'main.py -h'
