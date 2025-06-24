# Template project using imklib

## Fork, clone and run

```bash
git clone https://github.com/<user>/<fork>.git my-project
cd my-project
git submodule update --remote --merge
mkdir -p deps/imklib/build
cd deps/imklib/build
cmake ..
make
cd -
mkdir build
ln -rs build/compile_commands.json compile_commands.json
cd build
cmake -DCMAKE_EXPORT_COMPILE_COMMANDS=ON ..
make
./main
```
