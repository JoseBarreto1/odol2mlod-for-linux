# odol2mlodForLinux


## ✅ Etapas para compilar e usar o odol2mlod no Linux

🛠️ 1. Verifique se você tem as dependências:

- Como o projeto é em C++ com CMake, você vai precisar de:

```
sudo apt install build-essential cmake
```

📁 2. Compile o projeto
- Navegue até a pasta do projeto:

```
cd /caminho/para/odol2mlod
```
- Crie um diretório de build e compile:

```
mkdir build
cd build
cmake ..
make
```

🚀 3. Como usar o odol2mlod
## ✅ Sintaxe básica:

```
./odol2mlod modelo.p3d
```

Isso gera: modelo_mlod.p3d (uma cópia convertida)

# 📚 Exemplos com flags úteis:

- Merge total de vértices:
```
./odol2mlod -m modelo.p3d
```

- Info completa do .p3d:
```
./odol2mlod -I modelo.p3d
```

- Lista de texturas usadas no modelo:
```
./odol2mlod -t modelo.p3d
```

- Conversão em lote recursiva (diretório inteiro):
```
./odol2mlod -r pasta_com_p3d/
```

- Exemplo completo com várias flags:
```
./odol2mlod -sirt pasta_com_p3d/
```

## Explicando as flags:

-s → gera um único arquivo .txt com os dados

-i → gera informações básicas do modelo

-r → procura .p3d recursivamente

-t → gera lista de texturas

# Extras:

Converts 3D models (.P3D extension) for the video game [Operation Flashpoint](https://en.wikipedia.org/wiki/Operation_Flashpoint:_Cold_War_Crisis) (also known as ArmA: Cold War Assault) from the [ODOL v7](https://community.bistudio.com/wiki/P3D_File_Format_-_ODOLV7) to the [MLOD](https://community.bistudio.com/wiki/P3D_File_Format_-_MLOD) SP3X format.

Coded by Miki. Additional options by [Faguss](https://ofp-faguss.com).

Build files generated with CMake 3.27.6. Compiled with gcc (x86_64-win32-seh-rev0, Built by MinGW-W64 project) 8.1.0

Binary and readme: https://ofp-faguss.com/odol2mlod or see [releases](https://github.com/Faguss/odol2mlod/releases)
