# BindingGenerator
Generate Python or Lua bindings.

Currently the generator produces Boost Python bindings. To run the generator:
1. Install CLANG 32 bit.
2. Create an environment variable called CLANG_PATH and set it to the LLVM/bin folder in which the libclang.dll file is present.
2. Install Python 2.7 32 bit.
3. Install Python Tools for Visual Studio(not necessary but useful). The solution file is for Visual Studio 2013.
4. Open the CPPBindingGenerator.sln solution.
5. In the Solution Explorer under Python environments, Python 2.7 should be highlighted. Right click the node & Install Python Package - install clang & Mako.
6. Run CPPBindingGenerator.py.
7. The project passes the 'TextComponent.h' as a the first command line argument which is the input file to scan. The Python bindings appear in textcomponent_bind.h in the same directory.
8. Enjoy!

Lua bindings support using luabind will be added soon. 

