# Extractor-.SCS-files-mods
Extractor .SCS files mods Euro Truck Simulator 2

scs_to_blender.py é o código-fonte, na versão 1.5.
README.md, em português com um resumo em inglês, traz:
os recursos e uma tabela de formatos suportados;
as instruções de uso (.exe, Python e linha de comando);
dicas para o Blender e um resumo de como funciona;
uma seção de uso responsável e a licença.
docs/FORMATS.md documenta os formatos que descobrimos nas conversas: HashFS v1 e CityHash64, o ZIP lido só pelo diretório central, as três versões de PMG com as tabelas de offsets, PMD, materiais e texturas, e o glTF de saída.
tests/test_core.py tem 13 testes offline, sem arquivos do jogo. Eles geram PMG 0x13 e 0x15 sintéticos e cobrem o hash, o GLB, os tipos de pacote e a conversão ponta a ponta.
.github/workflows/build.yml roda os testes e compila SCS2Blender.exe e SCS2Blender_console.exe. Ao criar uma tag v*, ele anexa os dois ao Release.
Os scripts .bat e .ps1 de build sem Python, requirements.txt e requirements-build.txt.
CHANGELOG.md (versões 1.0 a 1.5), CONTRIBUTING.md, LICENSE (MIT) e .gitignore.

scs_to_blender.py` is the source code (version 1.5).
`README.md`—written in Portuguese with an English summary—includes:
features and a table of supported formats;
usage instructions (for the .exe, Python, and command line);
tips for Blender and an overview of how the tool works;
a section on responsible use, as well as the license.
`docs/FORMATS.md` documents the formats identified during our discussions: HashFS v1 and CityHash64; ZIP files read via the central directory; three versions of PMG (including offset tables), PMD, materials, and textures; and the output glTF format.
`tests/test_core.py` contains 13 offline tests that do not require game files. These generate synthetic PMG 0x13 and 0x15 files, covering hashing, GLB generation, package types, and end-to-end conversion.
`.github/workflows/build.yml` runs the tests and compiles `SCS2Blender.exe` and `SCS2Blender_console.exe`. When a `v*` tag is created, it attaches both executables to the release.
The repository also includes `.bat` and `.ps1` scripts for building without a Python installation, along with `requirements.txt` and `requirements-build.txt`.
Also included are `CHANGELOG.md` (covering versions 1.0 through 1.5), `CONTRIBUTING.md`, the license (MIT), and `.gitignore`.
