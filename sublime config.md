sublime config

https://www.jianshu.com/p/8ba3aebf921c

sublimeREPL need sudo

{
	"command": "repl_open",
    "caption": "Python - RUN current file",
    "id": "repl_python_run",
    "mnemonic": "R",
    "args": 
    {
        "type": "subprocess",
        "encoding": "utf8",
        "cmd": ["sudo", "-S", "/usr/bin/python3.6", "-u", "$file_basename"],
        "cwd": "$file_path",
        "syntax": "Packages/Python/Python.tmLanguage",
        "external_id": "python",
        "extend_env": {"PYTHONIOENCODING": "utf-8"}
    }
},