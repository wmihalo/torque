include ../Makefile.ut

libuut_la_SOURCES =  ${PROG_ROOT}/req_runjob.c

coverage_run.sh:
	echo 'cp -p .libs/req_runjob.gc* . >/dev/null 2>&1' > $@
	echo 'RESULTS=($$(gcov req_runjob.gcda))' >> $@
	echo 'PARSED_RESULT="TOTALCOV -- $${RESULTS[1]}: Lines($${RESULTS[5]})- $${RESULTS[3]}"' >> $@
	echo 'echo -e "\033[40m\033[1;33m$$PARSED_RESULT\033[0m"' >> $@
	chmod +x $@
