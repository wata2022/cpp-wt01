# このプロジェクトをビルドするために必要なCMakeの最低バージョンを指定します。
# これより古いバージョンのCMakeではビルドできません。
cmake_minimum_required(VERSION 3.20)

# プロジェクトの名前を「cpp_hello_world」と定義し、言語としてC++ (CXX) を指定します。
project(cpp_hello_world CXX)

# 使用するC++の標準バージョンを「17」(C++17) に設定します。
set(CMAKE_CXX_STANDARD 17)

# 上記で設定したC++標準のバージョンを使用することを必須とします。
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# 「main.cpp」ソースファイルから「main」という名前の実行可能ファイルを生成するよう指示します。
# Windowsでは「main.exe」という名前のファイルが作成されます。
add_executable(main main.cpp)