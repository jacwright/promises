exec = require('child_process').exec
spawn = require('child_process').spawn


task 'compile', 'Compile to Javascript', ->
	start = new Date().getTime()
	exec 'coffee -c lib/promises', (error, stdout, stderr) ->
		console.error error if error?
		console.error stderr if stderr
		console.log stdout if stdout
		console.log "Compiled in #{new Date().getTime() - start} ms" if not error
