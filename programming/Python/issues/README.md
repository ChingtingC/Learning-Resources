* Message: zsh: illegal hardware instruction  python
    * cause: MacOS M1
    * solution: https://github.com/apple/tensorflow_macos/issues/153
    * steps:
        1. `xcode-select --install`
        2. Use `which xcrun` to check installation of xcode
            * output: `/usr/bin/xcrun`
        3. install [miniforge3](https://github.com/conda-forge/miniforge#miniforge3) for system's architecture 
        4. Use `file $(which python)` to check installation of miniforge
            * output: `<your home dir>/miniforge3/bin/python: Mach-O 64-bit executable arm64`
        5. Use `which pip` to check installation of miniforge
            * output: `<your home dir>/miniforge3/bin/pip`
        6. Download [environment.yml](https://raw.githubusercontent.com/mwidjaja1/DSOnMacARM/main/environment.yml)
        7. `conda env create --file=PATH_TO_ENVIRONMENT.YML --name=YOUR_ENV_NAME_HERE`
        8. `conda activate YOUR_ENV_NAME_HERE`
        10. `pip install --upgrade --force --no-dependencies https://github.com/apple/tensorflow_macos/releases/download/v0.1alpha3/tensorflow_macos-0.1a3-cp38-cp38-macosx_11_0_arm64.whl https://github.com/apple/tensorflow_macos/releases/download/v0.1alpha3/tensorflow_addons_macos-0.1a3-cp38-cp38-macosx_11_0_arm64.whl`
        11. Done :D
