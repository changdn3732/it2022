ARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
boot@boot-Default-string:~/lab_control_app/lab_control_app$ .run.sh
.run.sh: command not found
boot@boot-Default-string:~/lab_control_app/lab_control_app$ ./run.sh
bash: ./run.sh: No such file or directory
boot@boot-Default-string:~/lab_control_app/lab_control_app$ cd ..
boot@boot-Default-string:~/lab_control_app$ ./run.sh
Traceback (most recent call last):
  File "/home/boot/lab_control_app/lab_control_app/main.py", line 72, in <module>
    ft.run(target=main)
TypeError: run() missing 1 required positional argument: 'main'
boot@boot-Default-string:~/lab_control_app$ cd /lab_control_app
bash: cd: /lab_control_app: No such file or directory
boot@boot-Default-string:~/lab_control_app$ cd /lab_control_app
bash: cd: /lab_control_app: No such file or directory
boot@boot-Default-string:~/lab_control_app$ cd lab_control_app
boot@boot-Default-string:~/lab_control_app/lab_control_app$ ./run.sh
./run.sh: line 30: cd: lab_control_app: No such file or directory
Traceback (most recent call last):
  File "/home/boot/lab_control_app/lab_control_app/main.py", line 72, in <module>
    ft.run(target=main)
TypeError: run() missing 1 required positional argument: 'main'
boot@boot-Default-string:~/lab_control_app/lab_control_app$ 
