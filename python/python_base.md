##Python执行系统命令的方法 os.system()，os.popen()，commands

	>>> os.system('ls .')
	python-note.md python_base.md
	0
	>>> (status, output) = commands.getstatusoutput('cat /proc/cpuinfo')
	>>> output = os.popen('cat /proc/cpuinfo')
	print output.read()
