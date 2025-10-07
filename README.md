# pip_install_requirements_debugger
when i install rvc requirements.txt today(20250929), i failed, so i wrote this script for me.

# Usage
```
python idebug.py requirements.txt
```

# Example
```
(C:\ai) C:\Users\原神>python "C:\Users\原神\Desktop\idebug.py" "C:\Users\原神\Desktop\requirements.txt"
pip install aria2

    STDOUT: Requirement already satisfied: aria2 in c:\ai\lib\site-packages (0.0.1b0)

    STDERR: EMPTY


pip install joblib

    STDOUT: Requirement already satisfied: joblib in c:\ai\lib\site-packages (1.5.2)

    STDERR: EMPTY


pip install numba

    STDOUT: Requirement already satisfied: numba in c:\ai\lib\site-packages (0.62.0)
Requirement already satisfied: llvmlite<0.46,>=0.45.0dev0 in c:\ai\lib\site-packages (from numba) (0.45.0)
Requirement already satisfied: numpy<2.4,>=1.22 in c:\ai\lib\site-packages (from numba) (1.26.4)

    STDERR: EMPTY


pip install numpy

    STDOUT: Requirement already satisfied: numpy in c:\ai\lib\site-packages (1.26.4)

    STDERR: EMPTY


pip install scipy

    STDOUT: Requirement already satisfied: scipy in c:\ai\lib\site-packages (1.15.3)
Requirement already satisfied: numpy<2.5,>=1.23.5 in c:\ai\lib\site-packages (from scipy) (1.26.4)

    STDERR: EMPTY


pip install librosa

    STDOUT: Collecting librosa
  Using cached librosa-0.11.0-py3-none-any.whl.metadata (8.7 kB)
Collecting audioread>=2.1.9 (from librosa)
  Using cached audioread-3.0.1-py3-none-any.whl.metadata (8.4 kB)
Requirement already satisfied: numba>=0.51.0 in c:\ai\lib\site-packages (from librosa) (0.62.0)
Requirement already satisfied: numpy>=1.22.3 in c:\ai\lib\site-packages (from librosa) (1.26.4)
Requirement already satisfied: scipy>=1.6.0 in c:\ai\lib\site-packages (from librosa) (1.15.3)
Collecting scikit-learn>=1.1.0 (from librosa)
  Using cached scikit_learn-1.7.2-cp310-cp310-win_amd64.whl.metadata (11 kB)
Requirement already satisfied: joblib>=1.0 in c:\ai\lib\site-packages (from librosa) (1.5.2)
Collecting decorator>=4.3.0 (from librosa)
  Using cached decorator-5.2.1-py3-none-any.whl.metadata (3.9 kB)
Collecting soundfile>=0.12.1 (from librosa)
  Using cached soundfile-0.13.1-py2.py3-none-win_amd64.whl.metadata (16 kB)
Collecting pooch>=1.1 (from librosa)
  Using cached pooch-1.8.2-py3-none-any.whl.metadata (10 kB)
Collecting soxr>=0.3.2 (from librosa)
  Using cached soxr-1.0.0-cp310-cp310-win_amd64.whl.metadata (5.6 kB)
Requirement already satisfied: typing_extensions>=4.1.1 in c:\ai\lib\site-packages (from librosa) (4.15.0)
Collecting lazy_loader>=0.1 (from librosa)
  Using cached lazy_loader-0.4-py3-none-any.whl.metadata (7.6 kB)
Collecting msgpack>=1.0 (from librosa)
  Using cached msgpack-1.1.1-cp310-cp310-win_amd64.whl.metadata (8.6 kB)
Requirement already satisfied: packaging in c:\ai\lib\site-packages (from lazy_loader>=0.1->librosa) (25.0)
Requirement already satisfied: llvmlite<0.46,>=0.45.0dev0 in c:\ai\lib\site-packages (from numba>=0.51.0->librosa) (0.45.0)
Requirement already satisfied: platformdirs>=2.5.0 in c:\ai\lib\site-packages (from pooch>=1.1->librosa) (4.4.0)
Requirement already satisfied: requests>=2.19.0 in c:\ai\lib\site-packages (from pooch>=1.1->librosa) (2.32.5)
Requirement already satisfied: charset_normalizer<4,>=2 in c:\ai\lib\site-packages (from requests>=2.19.0->pooch>=1.1->librosa) (3.4.3)
Requirement already satisfied: idna<4,>=2.5 in c:\ai\lib\site-packages (from requests>=2.19.0->pooch>=1.1->librosa) (3.10)
Requirement already satisfied: urllib3<3,>=1.21.1 in c:\ai\lib\site-packages (from requests>=2.19.0->pooch>=1.1->librosa) (2.5.0)
Requirement already satisfied: certifi>=2017.4.17 in c:\ai\lib\site-packages (from requests>=2.19.0->pooch>=1.1->librosa) (2025.8.3)
Collecting threadpoolctl>=3.1.0 (from scikit-learn>=1.1.0->librosa)
  Downloading threadpoolctl-3.6.0-py3-none-any.whl.metadata (13 kB)
Requirement already satisfied: cffi>=1.0 in c:\ai\lib\site-packages (from soundfile>=0.12.1->librosa) (2.0.0)
Requirement already satisfied: pycparser in c:\ai\lib\site-packages (from cffi>=1.0->soundfile>=0.12.1->librosa) (2.22)
Downloading librosa-0.11.0-py3-none-any.whl (260 kB)
Downloading audioread-3.0.1-py3-none-any.whl (23 kB)
Using cached decorator-5.2.1-py3-none-any.whl (9.2 kB)
Downloading lazy_loader-0.4-py3-none-any.whl (12 kB)
Downloading msgpack-1.1.1-cp310-cp310-win_amd64.whl (71 kB)
Downloading pooch-1.8.2-py3-none-any.whl (64 kB)
Downloading scikit_learn-1.7.2-cp310-cp310-win_amd64.whl (8.9 MB)
   ---------------------------------------- 8.9/8.9 MB 19.7 MB/s  0:00:00
Downloading soundfile-0.13.1-py2.py3-none-win_amd64.whl (1.0 MB)
   ---------------------------------------- 1.0/1.0 MB 16.1 MB/s  0:00:00
Downloading soxr-1.0.0-cp310-cp310-win_amd64.whl (173 kB)
Downloading threadpoolctl-3.6.0-py3-none-any.whl (18 kB)
Installing collected packages: threadpoolctl, soxr, msgpack, lazy_loader, decorator, audioread, soundfile, scikit-learn, pooch, librosa

Successfully installed audioread-3.0.1 decorator-5.2.1 lazy_loader-0.4 librosa-0.11.0 msgpack-1.1.1 pooch-1.8.2 scikit-learn-1.7.2 soundfile-0.13.1 soxr-1.0.0 threadpoolctl-3.6.0

    STDERR: EMPTY


pip install llvmlite

    STDOUT: Requirement already satisfied: llvmlite in c:\ai\lib\site-packages (0.45.0)

    STDERR: EMPTY


pip install fairseq

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Error occurred:
fairseq
STDOUT: Collecting fairseq
  Using cached fairseq-0.12.2.tar.gz (9.6 MB)
  Installing build dependencies: started
  Installing build dependencies: still running...
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'done'
  Installing backend dependencies: started
  Installing backend dependencies: still running...
  Installing backend dependencies: finished with status 'done'
  Preparing metadata (pyproject.toml): started
  Preparing metadata (pyproject.toml): finished with status 'done'
Requirement already satisfied: cffi in c:\ai\lib\site-packages (from fairseq) (2.0.0)
Collecting cython (from fairseq)
  Using cached cython-3.1.4-cp310-cp310-win_amd64.whl.metadata (5.1 kB)
Collecting hydra-core<1.1,>=1.0.7 (from fairseq)
  Using cached hydra_core-1.0.7-py3-none-any.whl.metadata (3.7 kB)
Collecting omegaconf<2.1 (from fairseq)
  Using cached omegaconf-2.0.6-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.5-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.4-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.3-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.2-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.1-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.0-py3-none-any.whl.metadata (3.5 kB)
Requirement already satisfied: numpy in c:\ai\lib\site-packages (from fairseq) (1.26.4)
Collecting regex (from fairseq)
  Using cached regex-2025.9.18-cp310-cp310-win_amd64.whl.metadata (41 kB)
Collecting sacrebleu>=1.4.12 (from fairseq)
  Using cached sacrebleu-2.5.1-py3-none-any.whl.metadata (51 kB)
Requirement already satisfied: torch in c:\ai\lib\site-packages (from fairseq) (2.5.1)
Requirement already satisfied: tqdm in c:\ai\lib\site-packages (from fairseq) (4.67.1)
Collecting bitarray (from fairseq)
  Using cached bitarray-3.7.1-cp310-cp310-win_amd64.whl.metadata (35 kB)
Requirement already satisfied: torchaudio>=0.8.0 in c:\ai\lib\site-packages (from fairseq) (2.5.1)
Collecting omegaconf<2.1 (from fairseq)
  Using cached omegaconf-2.0.6-py3-none-any.whl.metadata (3.0 kB)
  Using cached omegaconf-2.0.5-py3-none-any.whl.metadata (3.0 kB)
INFO: pip is looking at multiple versions of hydra-core to determine which version is compatible with other requirements. This could take a while.
Collecting fairseq
  Using cached fairseq-0.12.1.tar.gz (9.6 MB)
  Installing build dependencies: started
  Installing build dependencies: still running...
  Installing build dependencies: finished with status 'done'
  Getting requirements to build wheel: started
  Getting requirements to build wheel: finished with status 'error'

STDERR: WARNING: Ignoring version 2.0.6 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/d0/eb/9d63ce09dd8aa85767c65668d5414958ea29648a0eec80a4a7d311ec2684/omegaconf-2.0.6-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.5 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/e5/f6/043b6d255dd6fbf2025110cea35b87f4c5100a181681d8eab496269f0d5b/omegaconf-2.0.5-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.4 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/92/b1/4f3023143436f12c98bab53f0b3db617bd18a7d223627d5030e13a7b4fc2/omegaconf-2.0.4-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.3 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/29/08/a88210c2c1aa0a3f65f05d8a6c98939ccb84b6fb982aa6567dec4e6773f9/omegaconf-2.0.3-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.2 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/72/fe/f8d162aa059fb4f327fd75144dd69aa7e8acbb6d8d37013e4638c8490e0b/omegaconf-2.0.2-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.1 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/86/ec/605805e60abdb025b06664d107335031bb8ebdc52e0a90bdbad6a7130279/omegaconf-2.0.1-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.6 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/d0/eb/9d63ce09dd8aa85767c65668d5414958ea29648a0eec80a4a7d311ec2684/omegaconf-2.0.6-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
WARNING: Ignoring version 2.0.5 of omegaconf since it has invalid metadata:
Requested omegaconf<2.1 from https://files.pythonhosted.org/packages/e5/f6/043b6d255dd6fbf2025110cea35b87f4c5100a181681d8eab496269f0d5b/omegaconf-2.0.5-py3-none-any.whl (from fairseq) has invalid metadata: .* suffix can only be used with `==` or `!=` operators
    PyYAML (>=5.1.*)
            ~~~~~~^
Please use pip<24.1 if you need to use this version.
  error: subprocess-exited-with-error

  Getting requirements to build wheel did not run successfully.
  exit code: 1

  [16 lines of output]
  Traceback (most recent call last):
    File "C:\ai\lib\site-packages\pip\_vendor\pyproject_hooks\_in_process\_in_process.py", line 389, in <module>
      main()
    File "C:\ai\lib\site-packages\pip\_vendor\pyproject_hooks\_in_process\_in_process.py", line 373, in main
      json_out["return_val"] = hook(**hook_input["kwargs"])
    File "C:\ai\lib\site-packages\pip\_vendor\pyproject_hooks\_in_process\_in_process.py", line 143, in get_requires_for_build_wheel
      return hook(config_settings)
    File "C:\Users\原神\AppData\Local\Temp\pip-build-env-0lkcr3ee\overlay\Lib\site-packages\setuptools\build_meta.py", line 331, in get_requires_for_build_wheel
      return self._get_build_requires(config_settings, requirements=[])
    File "C:\Users\原神\AppData\Local\Temp\pip-build-env-0lkcr3ee\overlay\Lib\site-packages\setuptools\build_meta.py", line 301, in _get_build_requires
      self.run_setup()
    File "C:\Users\原神\AppData\Local\Temp\pip-build-env-0lkcr3ee\overlay\Lib\site-packages\setuptools\build_meta.py", line 317, in run_setup
      exec(code, locals())
    File "<string>", line 27, in <module>
    File "<string>", line 18, in write_version_py
  FileNotFoundError: [Errno 2] No such file or directory: 'fairseq\\version.txt'
  [end of output]

  note: This error originates from a subprocess, and is likely not a problem with pip.
error: subprocess-exited-with-error

Getting requirements to build wheel did not run successfully.
exit code: 1

See above for output.

note: This error originates from a subprocess, and is likely not a problem with pip.


(C:\ai) C:\Users\原神>
```

## The solution for install rvc failed above
https://github.com/facebookresearch/fairseq/issues/5511#issuecomment-2343923840<br>
https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/issues/1103#issuecomment-1697800003<br>
https://github.com/oobabooga/text-generation-webui/issues/3261#issuecomment-2614447205<br>
https://github.com/gradio-app/gradio/issues/6339#issue-1982978174<br>
https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/issues/2411#issuecomment-2566927653<br>
https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI/issues/2227#issuecomment-2286582025

## What I change for rvc script in my computer
```
#in cmd
set USE_LIBUV=0
set KMP_DUPLICATE_LIB_OK=TRUE

#in infer-web.py: remove concurrency_count argument
```

# sdebug.py
## if after install some package, torch will be break, and you don't know what package do
This script write by me because after install some package, my torch break, i cannot import torch, and search network, no anwser, so i recreate env and clone env, then use this script test.
### Usage
```cmd
python sdebug.py requirements.txt bug.py
rem bug.py will throw if there is a bug
rem sdebug.py will detect bug
```
#### custom bug.py
bug.py structure
```py
#This script will be error after some package install
#We need to find that package is what
#This script use by sdebug.py
# The code will put below
import torch
# The code will put above
#if nothing happen, no error, then output No bug.
print("No Bug.")
```

# Some other errors record
## Error1 Record
```cmd
C:\Users\原神>D:

D:\>conda activate D://aii

(D:\aii) D:\>python "C:\Users\原神\Desktop\神秘資料夾\idebug.py" "C:\Users\原神\Downloads\requirements (1).txt"
pip install diffusers>=0.32.1

    STDOUT:
    STDERR: EMPTY


pip install accelerate>=1.1.1

    STDOUT:
    STDERR: EMPTY


pip install transformers>=4.46.2

    STDOUT:
    STDERR: EMPTY


pip install numpy==1.26.0

    STDOUT: Collecting numpy==1.26.0
  Downloading numpy-1.26.0-cp310-cp310-win_amd64.whl.metadata (61 kB)
Downloading numpy-1.26.0-cp310-cp310-win_amd64.whl (15.8 MB)
   ---------------------------------------- 15.8/15.8 MB 25.5 MB/s  0:00:00
Installing collected packages: numpy
  Attempting uninstall: numpy
    Found existing installation: numpy 1.26.4
    Uninstalling numpy-1.26.4:
      Successfully uninstalled numpy-1.26.4
Successfully installed numpy-1.26.0

    STDERR: ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
opencv-contrib-python 4.12.0.88 requires numpy<2.3.0,>=2; python_version >= "3.9", but you have numpy 1.26.0 which is incompatible.
opencv-python 4.12.0.88 requires numpy<2.3.0,>=2; python_version >= "3.9", but you have numpy 1.26.0 which is incompatible.



pip install torch>=2.5.0

    STDOUT:
    STDERR: EMPTY


pip install torchvision>=0.20.0

    STDOUT:
    STDERR: EMPTY


pip install sentencepiece>=0.2.0

    STDOUT:
    STDERR: EMPTY


pip install SwissArmyTransformer>=0.4.12

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
Error occurred:
SwissArmyTransformer>=0.4.12
STDOUT:
STDERR:   error: subprocess-exited-with-error

  python setup.py egg_info did not run successfully.
  exit code: 1

  [31 lines of output]
  test.c
  LINK : fatal error LNK1181: 無法開啟輸入檔 'aio.lib'
  Traceback (most recent call last):
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\op_builder\builder.py", line 405, in cpu_arch
      from cpuinfo import get_cpu_info
  ModuleNotFoundError: No module named 'cpuinfo'

  During handling of the above exception, another exception occurred:

  Traceback (most recent call last):
    File "<string>", line 2, in <module>
    File "<pip-setuptools-caller>", line 35, in <module>
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\setup.py", line 201, in <module>
      ext_modules.append(builder.builder())
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\op_builder\builder.py", line 713, in builder
      {'cxx': self.strip_empty_entries(self.cxx_args()), \
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\op_builder\builder.py", line 854, in cxx_args
      CPU_ARCH = self.cpu_arch()
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\op_builder\builder.py", line 407, in cpu_arch
      cpu_info = self._backup_cpuinfo()
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\op_builder\builder.py", line 439, in _backup_cpuinfo
      if not self.command_exists('lscpu'):
    File "C:\Users\原神\AppData\Local\Temp\pip-install-kth18s88\deepspeed_aecc237abedd4943a0419c3a01b0b14c\op_builder\builder.py", line 497, in command_exists
      result = subprocess.Popen(safe_cmd, stdout=subprocess.PIPE)
    File "D:\aii\lib\subprocess.py", line 971, in __init__
      self._execute_child(args, executable, preexec_fn, close_fds,
    File "D:\aii\lib\subprocess.py", line 1440, in _execute_child
      hp, ht, pid, tid = _winapi.CreateProcess(executable, args,
  FileNotFoundError: [WinError 2] 系統找不到指定的檔案。
  DS_BUILD_OPS=1
   [WARNING]  Skip pre-compile of incompatible async_io; One can disable async_io with DS_BUILD_AIO=0
  [end of output]

  note: This error originates from a subprocess, and is likely not a problem with pip.
error: metadata-generation-failed

Encountered error while generating package metadata.

See above for output.

note: This is an issue with the package mentioned above, not pip.
hint: See above for details.


(D:\aii) D:\>
```

### Prolbem
...so many...

https://github.com/zai-org/CogVideo/blob/main/requirements.txt

https://github.com/THUDM/SwissArmyTransformer/blob/main/requirements.txt

https://www.google.com/search?q=ModuleNotFoundError%3A+No+module+named+%27cpuinfo%27&oq=ModuleNotFoundError%3A+No+module+named+%27cpuinfo%27&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIGCAEQRRg6MgYIAhBFGDwyBggDEEUYPNIBBzQ1NmowajeoAgCwAgA&sourceid=chrome&ie=UTF-8

https://github.com/deepspeedai/DeepSpeed/issues/4669

https://www.google.com/search?q=ERROR%3A+Failed+building+wheel+for+deepspeed&oq=ERROR%3A+Failed+building+wheel+for+deepspeed&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIGCAEQRRg60gEHMjYwajBqN6gCALACAA&sourceid=chrome&ie=UTF-8

https://stackoverflow.com/questions/73264234/pytorch-error-checking-compiler-version-for-cl-cpp-extension-py

https://github.com/deepspeedai/DeepSpeed/issues/4729

https://github.com/deepspeedai/DeepSpeed/issues/3145

https://github.com/deepspeedai/DeepSpeed/blob/master/blogs/windows/08-2024/README.md

https://github.com/deepspeedai/DeepSpeed#windows

https://github.com/deepspeedai/DeepSpeed/issues/6923

https://www.google.com/search?q=No+module+named+build&oq=No+module+named+build&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIGCAEQABgeMgYIAhAAGB4yBggDEAAYHjIGCAQQABgeMgYIBRAAGB4yBggGEAAYHjIGCAcQABgeMggICBAAGAUYHjIICAkQABgFGB7SAQc0MTdqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8

### $${\color{red}Solution}$$
1. ```pip install py-cpuinfo```

2. https://stackoverflow.com/questions/73264234/pytorch-error-checking-compiler-version-for-cl-cpp-extension-py

<img width="877" height="462" alt="image" src="https://github.com/user-attachments/assets/607ceece-88fb-48e9-be94-9d2077ac7739" />

3. http://github.com/deepspeedai/DeepSpeed/blob/master/blogs/windows/08-2024/README.md#building-from-source

<img width="1121" height="225" alt="image" src="https://github.com/user-attachments/assets/7a85bf5c-77a9-42b4-8a6b-e38229327dc9" />


### $${\color{red}Problem2}$$
https://github.com/neonbjb/tortoise-tts/issues/556

### $${\color{red}Solution2}$$
https://github.com/neonbjb/tortoise-tts/issues/556#issuecomment-1883569462

<img width="926" height="433" alt="image" src="https://github.com/user-attachments/assets/f349ab98-44e2-460b-be07-cdc9d1392a35" />


### Finally
after success build and install deepspeed, run ```pip install SwissArmyTransformer``` success.


## Error2 Record
No moudle name torch in notebook? My problem is my notebook installed in computer, but not install in current conda env, so solution is ```pip install notebook```.
