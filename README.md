# autoDockVina
- Bash script for running a autoDock Vina job on a different system.
- As input the vina `vina_config.txt` file is required.
- The `path` of each file is changed to the current location and vina can be started.
- The script also adds a cofactor or ligand .pdbqt file to the receptor.rigid.pdbqt file. This is useful if a previous ligand should be included in a redocking with another ligand.

## Requirements
- AutoDock Vina (tested with 1.1.2; Ubuntu_16.04)
- For the `-l` flag the cofactor or ligand to add, has to be prepared with autoDockTools or has to be splitted with `vina_split` to have only one conformational state.

## Installation
- Bash script, just make it executable and run

### SourceCode compiling with Argbash - argument parser generator
- template file can be changed and converted to executable code (tested with argbash_2.8.1; Ubuntu_16.04)
- `argbash autoDockVina_template -o autoDockVina` 
