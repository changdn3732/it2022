sudo apt update && sudo apt install -y python3 python3-pip python3-venv \
    libgtk-3-0 libgstreamer1.0-0 libgstreamer-plugins-base1.0-0 \
    gstreamer1.0-plugins-good libmpv1 libglib2.0-0 libcairo2 \
    libpango-1.0-0 libpangocairo-1.0-0 git

# 시리얼 포트 권한
sudo usermod -a -G dialout $USER

# 프로젝트 클론 및 실행
git clone https://github.com/changdn3732/lab_control_app.git
cd lab_control_app
chmod +x run.sh
./run.sh
Hit:1 http://security.ubuntu.com/ubuntu jammy-security InRelease               
Hit:2 http://us.archive.ubuntu.com/ubuntu jammy InRelease                      
Hit:3 http://us.archive.ubuntu.com/ubuntu jammy-updates InRelease
Hit:4 http://us.archive.ubuntu.com/ubuntu jammy-backports InRelease
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
3 packages can be upgraded. Run 'apt list --upgradable' to see them.
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
libcairo2 is already the newest version (1.16.0-5ubuntu2).
libmpv1 is already the newest version (0.34.1-1ubuntu3).
git is already the newest version (1:2.34.1-1ubuntu1.15).
gstreamer1.0-plugins-good is already the newest version (1.20.3-0ubuntu1.4).
libglib2.0-0 is already the newest version (2.72.4-0ubuntu2.9).
libgstreamer-plugins-base1.0-0 is already the newest version (1.20.1-1ubuntu0.5).
libgstreamer1.0-0 is already the newest version (1.20.3-0ubuntu1.1).
libgtk-3-0 is already the newest version (3.24.33-1ubuntu2.2).
libpango-1.0-0 is already the newest version (1.50.6+ds-2ubuntu1).
libpangocairo-1.0-0 is already the newest version (1.50.6+ds-2ubuntu1).
python3 is already the newest version (3.10.6-1~22.04.1).
python3-pip is already the newest version (22.0.2+dfsg-1ubuntu0.7).
python3-venv is already the newest version (3.10.6-1~22.04.1).
The following packages were automatically installed and are no longer required:
  libwpe-1.0-1 libwpebackend-fdo-1.0-1
Use 'sudo apt autoremove' to remove them.
0 upgraded, 0 newly installed, 0 to remove and 3 not upgraded.
Cloning into 'lab_control_app'...
remote: Enumerating objects: 43, done.
remote: Counting objects: 100% (43/43), done.
remote: Compressing objects: 100% (34/34), done.
remote: Total 43 (delta 17), reused 34 (delta 8), pack-reused 0 (from 0)
Receiving objects: 100% (43/43), 48.61 KiB | 3.04 MiB/s, done.
Resolving deltas: 100% (17/17), done.
📦 패키지를 설치합니다... (sudo 권한 필요)
   (온라인 모드)
Collecting flet>=0.21.0
  Downloading flet-0.80.5-py3-none-any.whl (484 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 484.6/484.6 KB 10.9 MB/s eta 0:00:00
Collecting flet-charts>=0.1.0
  Downloading flet_charts-0.80.5-py3-none-any.whl (72 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 72.9/72.9 KB 21.8 MB/s eta 0:00:00
Collecting plotly>=5.0.0
  Downloading plotly-6.5.2-py3-none-any.whl (9.9 MB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 9.9/9.9 MB 73.8 MB/s eta 0:00:00
Collecting pymodbus>=3.0.0
  Downloading pymodbus-3.12.0-py3-none-any.whl (167 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 167.8/167.8 KB 45.6 MB/s eta 0:00:00
Collecting pyserial>=3.5
  Downloading pyserial-3.5-py2.py3-none-any.whl (90 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 90.6/90.6 KB 32.7 MB/s eta 0:00:00
Collecting httpx>=0.28.1
  Downloading httpx-0.28.1-py3-none-any.whl (73 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 73.5/73.5 KB 23.4 MB/s eta 0:00:00
Collecting oauthlib>=3.2.2
  Downloading oauthlib-3.3.1-py3-none-any.whl (160 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 160.1/160.1 KB 52.2 MB/s eta 0:00:00
Collecting repath>=0.9.0
  Downloading repath-0.9.0-py3-none-any.whl (4.7 kB)
Collecting typing-extensions
  Downloading typing_extensions-4.15.0-py3-none-any.whl (44 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 44.6/44.6 KB 12.8 MB/s eta 0:00:00
Collecting msgpack>=1.1.0
  Downloading msgpack-1.1.2-cp310-cp310-manylinux2014_x86_64.manylinux_2_17_x86_64.manylinux_2_28_x86_64.whl (406 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 406.1/406.1 KB 76.6 MB/s eta 0:00:00
Collecting narwhals>=1.15.1
  Downloading narwhals-2.16.0-py3-none-any.whl (443 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 444.0/444.0 KB 83.8 MB/s eta 0:00:00
Collecting packaging
  Downloading packaging-26.0-py3-none-any.whl (74 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 74.4/74.4 KB 22.6 MB/s eta 0:00:00
Collecting anyio
  Downloading anyio-4.12.1-py3-none-any.whl (113 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 113.6/113.6 KB 30.9 MB/s eta 0:00:00
Requirement already satisfied: certifi in /usr/lib/python3/dist-packages (from httpx>=0.28.1->flet>=0.21.0->-r lab_control_app/requirements.txt (line 1)) (2020.6.20)
Collecting httpcore==1.*
  Downloading httpcore-1.0.9-py3-none-any.whl (78 kB)
     ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 78.8/78.8 KB 28.0 MB/s eta 0:00:00
Requirement already satisfied: idna in /usr/lib/python3/dist-packages (from httpx>=0.28.1->flet>=0.21.0->-r lab_control_app/requirements.txt (line 1)) (3.3)
Collecting h11>=0.16
  Downloading h11-0.16.0-py3-none-any.whl (37 kB)
Requirement already satisfied: six>=1.9.0 in /usr/lib/python3/dist-packages (from repath>=0.9.0->flet>=0.21.0->-r lab_control_app/requirements.txt (line 1)) (1.16.0)
Collecting exceptiongroup>=1.0.2
  Downloading exceptiongroup-1.3.1-py3-none-any.whl (16 kB)
Installing collected packages: pyserial, typing-extensions, repath, pymodbus, packaging, oauthlib, narwhals, msgpack, h11, plotly, httpcore, exceptiongroup, anyio, httpx, flet, flet-charts
  Attempting uninstall: oauthlib
    Found existing installation: oauthlib 3.2.0
    Not uninstalling oauthlib at /usr/lib/python3/dist-packages, outside environment /usr
    Can't uninstall 'oauthlib'. No files were found to uninstall.
Successfully installed anyio-4.12.1 exceptiongroup-1.3.1 flet-0.80.5 flet-charts-0.80.5 h11-0.16.0 httpcore-1.0.9 httpx-0.28.1 msgpack-1.1.2 narwhals-2.16.0 oauthlib-3.3.1 packaging-26.0 plotly-6.5.2 pymodbus-3.12.0 pyserial-3.5 repath-0.9.0 typing-extensions-4.15.0
WARNING: Running pip as the 'root' user can result in broken permissions and conflicting behaviour with the system package manager. It is recommended to use a virtual environment instead: https://pip.pypa.io/warnings/venv
✅ 설치 완료!
/home/boot/lab_control_app/lab_control_app/main.py:72: DeprecationWarning: app() is deprecated since version 0.80.0. Use run() instead.
  ft.app(target=main)
Installing flet-desktop-light 0.80.5 package...OK
Traceback (most recent call last):
  File "/home/boot/lab_control_app/lab_control_app/main.py", line 72, in <module>
    ft.app(target=main)
  File "/usr/local/lib/python3.10/dist-packages/flet/utils/deprecated.py", line 40, in wrapper
    return func(*args, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/flet/app.py", line 43, in app
    return run(*new_args, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/flet/app.py", line 96, in run
    return asyncio.run(
  File "/usr/lib/python3.10/asyncio/runners.py", line 44, in run
    return loop.run_until_complete(main)
  File "/usr/lib/python3.10/asyncio/base_events.py", line 649, in run_until_complete
    return future.result()
  File "/usr/local/lib/python3.10/dist-packages/flet/app.py", line 224, in run_async
    from flet_desktop import close_flet_view, open_flet_view_async
ModuleNotFoundError: No module named 'flet_desktop'
